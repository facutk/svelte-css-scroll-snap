<script>
  import { onMount } from 'svelte';

  import cssScrollSnapPolyfill from 'css-scroll-snap-polyfill';

  onMount(cssScrollSnapPolyfill);
</script>

<main>
  <section id="home">
    <h2>home</h2>
  </section>
  <section id="tanguero">
    <h2>tanguero</h2>
  </section>
  <section id="flichman">
    <h2>flichman</h2>
  </section>
  <section id="misterio">
    <h2>misterio</h2>
  </section>
  <section id="caballero">
    <h2>caballero</h2>
  </section>
  <section id="dedicado">
    <h2>dedicado</h2>
  </section>
  <section id="bodega">
    <h2>bodega</h2>
  </section>
  <section id="consejos">
    <h2>consejos</h2>
  </section>
  <section id="contacto">
    <h2>Contacto</h2>
  </section>
</main>

<style>
  main {
    margin: 0 auto;
    max-height: 100vh;
    overflow-y: scroll;
    -ms-scroll-snap-type: mandatory;
    scroll-snap-type: mandatory;
    -ms-scroll-snap-points-y: repeat(100vh);
    scroll-snap-points-y: repeat(100vh);
    -ms-scroll-snap-type: y mandatory;
    scroll-snap-type: y mandatory;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }

  section {
    border-bottom: 1px dashed green;
    padding: 1rem;
    font-size: 1.2rem;
    color: red;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    scroll-snap-align: start;
    height: 100vh;
    width: 100vw;
  }
</style>