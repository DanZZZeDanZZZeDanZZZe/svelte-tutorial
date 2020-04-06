<script>
  import "../node_modules/materialize-css/dist/css/materialize.min.css";
  import "../node_modules/materialize-css/dist/js/materialize.min.js";

  import { Router, Link, Route } from "svelte-routing";

  import Navabr from "./layout/Navbar.svelte";

  import About from "./pages/About.svelte";
  import Home from "./pages/Home.svelte";
</script>

<Router>
  <Navabr />
  <div class="container">
    <Route path="/" component={Home} />
    <Route path="/about" component={About} />
  </div>
</Router>
