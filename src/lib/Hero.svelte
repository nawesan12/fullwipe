<script>
  import { fly } from "svelte/transition"

  let y
</script>

<svelte:window bind:scrollY={y} />

<section class="hero">
    <video class="hero-background" autoplay muted>
        <source src="/hero-background.mp4" type="video/mp4">
        <track kind="captions"/>
    </video>

    {#if y >= 0}
    <div class="hero-title">
        <img src="/images/logo.png" alt="Logo de Full Wipe" transition:fly="{{ x: -200, duration: 1200 }}">
        <h1 transition:fly="{{ x: 200, duration: 1000 }}">Full Wipe</h1>
        <h2 transition:fly="{{ y: 200, duration: 1000 }}">Limpieza Integral y Mantenimiento</h2>
    </div>
    {/if}
</section>

<style>
  .hero {
    max-width:100vw;
    max-height:90vh;
  }

  .hero-title {
    height:92vh;
    position: relative;
    z-index:5;
    color:#000;
    text-shadow: 0 0 4px var(--secondary);
    display:flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    text-align: center;
  }

  h1 {
    font-size:4.2rem;
  }

  h2 {
    font-size:2.5rem;
    font-weight:500;
  }

  img {
    height:12rem;
    padding: 0 0 7vh;
  }

  .hero-background {
    position:absolute;
    max-height:92vh;
    min-height:92vh;
    width:100vw;
    object-fit: cover;
    filter: brightness(1);
  }

  @media screen and (max-width:1200px) {
    .hero-title {
      margin-bottom:4rem;
      text-shadow: 0 0 2px rgb(255,255,255);
    }
  }
</style>
