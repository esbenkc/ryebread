<script>
  import { onMount } from "svelte";

  let images = [
    "https://madensverden.dk/wp-content/uploads/2021/08/hjemmebagt-kernerugbroed.jpg",
  ];

  //   Set a random initial poem
  let poem = poems[Math.floor(Math.random() * poems.length)];
  let image = images[Math.floor(Math.random() * images.length)];

  onMount(() => {
    setInterval(() => {
      poem = poems[Math.floor(Math.random() * poems.length)];
      image = images[Math.floor(Math.random() * images.length)];
    }, 10000);
  });
</script>

<svelte:head>
  <title>Ryebread {"<3"}</title>
  <meta
    name="description"
    content="Ryebread is a type of bread made with rye flour. It is usually denser and darker than bread made with wheat flour, and has a distinctive, slightly sour taste. Ryebread is popular in many European countries, particularly in Scandinavia and Germany."
  />
</svelte:head>

<section>
  <h1>Ryebread</h1>
  <span class="welcome">
    <picture>
      <img src={image} alt="Welcome" />
    </picture>
  </span>
  <p>Ryebread is very good.</p>
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    max-width: 900px;
    margin: 0 auto;
  }
  img {
    max-width: 400px;
  }
</style>
