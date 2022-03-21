<script>
  import Layout from './lib/Layout/Layout.svelte'
  import Hero from './lib/Hero.svelte'
  import ContactBanner from './lib/ContactBanner.svelte';
  import Services from './lib/Services.svelte';
  import Responsabilities from './lib/Responsabilities.svelte';
  import Materials from './lib/Materials.svelte';
  import CV from './lib/CV.svelte';
  import Contact from './lib/Contact.svelte';
</script>

<Layout>
  <Hero />
  <ContactBanner />
  <Services />
  <Materials />
  <Responsabilities />
  <CV />
  <Contact />
</Layout>

<style>
  :root {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen,
      Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;

    --primary: #5772ff;
    --secondary: #a3c3ff;
  }
  
  :global(*) {
    margin: 0;
    padding: 0;
  }

  :global(html) {
    scroll-behavior: smooth;
  }

  :global(body) {
    overflow-x: hidden;
  }

  :global(a) {
    color: #000;
    text-decoration: none;
  }

  :global(::-webkit-scrollbar) {
    width: 10px;
  }

  :global(::-webkit-scrollbar-track) {
    background: var(--secondary);
  }

  :global(::-webkit-scrollbar-thumb) {
    background: var(--primary);
  }

  :global(::-webkit-scrollbar-thumb:hover) {
    background:#5773ffb7;
  }
</style>