<script>
  import Mainpage from "./lib/Mainpage.svelte";
  import Underconstruction from "./lib/Underconstruction.svelte";
</script>

<main>
  <!-- remove overflow-hidden from index.html body -->
  <Underconstruction />
  <Mainpage />
</main>

<style>
  :root{
    background-color: #FFFDE7;
  }
</style>