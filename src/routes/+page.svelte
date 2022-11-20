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
      <img
        src="https://madensverden.dk/wp-content/uploads/2021/08/hjemmebagt-kernerugbroed.jpg"
        alt="Welcome"
      />
    </picture>
  </span>
  <p>Ryebread is very good.</p>
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    align-items: left;
    justify-content: center;
    max-width: 900px;
    margin: 0 auto;
  }
  h1 {
    font-size: 2.5rem;
    text-align: left;
  }

  img {
    max-width: 400px;
  }
</style>
