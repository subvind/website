<script>
  import { onMount } from "svelte";

  import Cradle from "./Cradle.svelte";
</script>

<div class="build-ideas">
  <div class="container">
    <br />
    <h1 class="title">
      WELCOME
    </h1>
    <div class="description" style="color: #fff;">
      We have a collection of "-nomy" modules for your website. Each module has a frontend main website and a backend admin panel. It integrates with your website by pointing your subdomain to a module's frontend; for example: store.istrav.com -> the erpnomy module. We currently have 1 module ready for production, 3 modules in development, and many more modules planned. Find out more by getting started today! Checkout our solutions and be sure to let us know how we are doing.
    </div>
    <!-- <br /> -->
    <!-- <div class="description">isTrav's goal is to solve problems using the right solutions, turn ideas into modules that spark joy to the end user, and then to keep production live with what works best.</div> -->
    <br />
    <a href="/solutions" class="btn btn-large red lighten-2"><i class="material-icons left">directions</i> GET STARTED!</a>
    <br />
    <br />
  </div>
  <br />
</div>
<div style="text-align: center;">
  <Cradle />
</div>

<style>
  .build-ideas {
    border-bottom: 1em solid #ee6e73;
    background-color: #222222;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 80 80' width='80' height='80'%3E%3Cpath fill='%23333333' fill-opacity='1' d='M14 16H9v-2h5V9.87a4 4 0 1 1 2 0V14h5v2h-5v15.95A10 10 0 0 0 23.66 27l-3.46-2 8.2-2.2-2.9 5a12 12 0 0 1-21 0l-2.89-5 8.2 2.2-3.47 2A10 10 0 0 0 14 31.95V16zm40 40h-5v-2h5v-4.13a4 4 0 1 1 2 0V54h5v2h-5v15.95A10 10 0 0 0 63.66 67l-3.47-2 8.2-2.2-2.88 5a12 12 0 0 1-21.02 0l-2.88-5 8.2 2.2-3.47 2A10 10 0 0 0 54 71.95V56zm-39 6a2 2 0 1 1 0-4 2 2 0 0 1 0 4zm40-40a2 2 0 1 1 0-4 2 2 0 0 1 0 4zM15 8a2 2 0 1 0 0-4 2 2 0 0 0 0 4zm40 40a2 2 0 1 0 0-4 2 2 0 0 0 0 4z'%3E%3C/path%3E%3C/svg%3E");
	}
  .build-ideas .title {
    font-weight: 900;
    font-size: 4.5em;
    text-align: left;
    margin: 0;
    color: #fff;
  }
  .build-ideas .description {
    color: #ccc;
    font-size: 1.5em;
  }
  .container {
    padding: 2em 0;
  }
</style>