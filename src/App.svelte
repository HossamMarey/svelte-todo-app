
<script>
  import {Router , Route} from 'svelte-navigator'
  import TodosPage from "./pages/TodosPage.svelte";
  import Header from "./components/layout/Header.svelte";
  import AboutPage from "./pages/AboutPage.svelte";
  import Posts from "./pages/Posts.svelte";
</script>


<div class="App">
  <Header />
  <!-- <TodosPage /> -->
  
  <Router>
    <Route path='/' component={TodosPage}/>
    <Route path='/about' component={AboutPage}/>
    <Route path='/posts/:id' component={Posts}/>
  </Router>

</div>