<script>
  import favicon from "$lib/assets/favicon.svg";

  let { children } = $props();
  import "../app.css";

  import Navbar from "../components/navbar.svelte";
</script>

<svelte:head>
  <link rel="icon" href={favicon} />
</svelte:head>

<Navbar />

{@render children?.()}
