<script>
  import Layout from './lib/Layout.svelte'
  import Hero from './lib/Hero.svelte'
</script>

<Layout>
  <Hero />
</Layout>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }
  
  :global(body) {
    overflow-x: hidden;
  }

  :global(*) {
    margin: 0;
    padding: 0;
  }

  :global(a) {
    color: #000;
    text-decoration: none;
  }
</style>


<!--
  rgb(87,114,255)
--> 