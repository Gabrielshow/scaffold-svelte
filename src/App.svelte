<script>
  import { Router, Route, Link } from 'svelte-routing';
  import Page from './Page.svelte';
  import About from './About.svelte';
  import HomePage from './HomePage.svelte';
</script>

<Router>
    <Route path="/" component={HomePage} />
    <Route path="/page" component={Page} />
    <Route path="/about" component={About} />
</Router>
