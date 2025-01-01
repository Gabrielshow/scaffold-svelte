<script>
  import { Router, Route, Link } from 'svelte-routing';
  import Page1 from './Page1.svelte';
  import Page2 from './Page2.svelte';
</script>

<style>
  /* Global styles for the app */
  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 10px;
    height: 100vh;
    width: 100%;
  }

  .logo {
    width: 200px;
    height: 200px;
    margin-bottom: 10px;
  }

  .black {
    color: black;
    margin: 0;
    text-align: center;
  }

  .redirect {
    background: black;
    width: 400px;
    color: white;
    border-radius: 2px;
    cursor: pointer;
    border: none;
    height: 40px;
    margin-right: 10px;
    margin-left: 10px;
    transform: opacity 0.3s ease-in, box-shadow 0.3s ease-in;
  }

  .redirect:hover {
    opacity: 0.8;
    box-shadow: 1px 1px 1px 1px grey;
  }
</style>

<Router>
  <div class="container">
    <div>
      <img class="logo" src="/assets/bell.png" alt="bell"/>
    </div>
    <h1 class="black">Your e-bill is Ready for review</h1>
    <Link to="/page1">
      <button class="redirect">Go to Page 1</button>
    </Link>
    <Link to="/page2">
      <button class="redirect">Go to Page 2</button>
    </Link>

    <Route path="/page1" component={Page1} />
    <Route path="/page2" component={Page2} />
  </div>
</Router>
