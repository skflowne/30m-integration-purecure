<script>
  import Tailwindcss from "./Tailwindcss.svelte";
  import Sidebar from "./components/Sidebar.svelte";
  import MainBlock from "./components/MainBlock.svelte";
</script>

<style global>
  a {
    text-decoration: none;
  }

  html {
    height: 100vh;
  }

  body {
    min-height: 100%;
    padding: 5%;
    background-color: #cddbfd;
  }

  .app {
    min-height: 90%;
    height: 90%;
    background: #fff;
    border-radius: 20px;
  }
</style>

<Tailwindcss />

<div class="app shadow-xl flex flex-row">
  <Sidebar />
  <MainBlock />
</div>
