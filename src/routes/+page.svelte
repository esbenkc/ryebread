<script>
  import { onMount } from "svelte";
  const imgs = [
    "https://nordicfoodliving.com/wp-content/uploads/2015/09/20198183221_eb41aa8508_b.jpg",
    "https://images.arla.com/recordid/615B5FD4-8460-4DED-BFE66F26326C100F/hurtigt-rugbrod.jpg?width=375&height=265&mode=crop",
    "https://889755.smushcdn.com/2066490/wp-content/uploads/2020/05/IMG_0125-750x926.jpg?lossy=1&strip=1&webp=1",
    "https://dk-spisbedre-production.imgix.net/images/recipes/hjemmebagt-rugbrod-med-hvidtol_14543.jpg?fit=crop&crop=focalpoint&fp-x=0.5&fp-y=0.5&fp-z=1.0w=1200&h=628",
    "https://madensverden.dk/wp-content/uploads/2021/08/hjemmebagt-kernerugbroed.jpg",
    "https://images.squarespace-cdn.com/content/v1/5bd5aeff77b903078e07ecd9/1540732332121-8UMVHUPZ78KTSOGJGN0W/IMG_2860.jpg",
    "https://opskrifteradmin.coop.dk/media/recipeimages/5107/20506/1920/rugbroed_agurk_hytteost.jpg?width=850&upscale=false&format=jpg&quality=90",
    "https://dk-spisbedre-production.imgix.net/images/recipes/fuldkornsrugbrod-uden-surdej_2598.jpg?fit=crop&crop=focalpoint&fp-x=0.4631067961165&fp-y=0.473059058817&fp-z=1.0796645702306&w=1200&h=628",
    "https://meyers.dk/media/12700/moerktkernerudbroed_meyersglutenfri_3_0377.jpg?anchor=center&mode=crop&width=1260&format=jpeg&quality=80&rnd=132151022390000000",
    "https://groedgrisen.dk/wp-content/uploads/2018/09/hjemmebagt-rugbroed-med-kerner-groft-sundt-4.jpg",
    "https://www.daringgourmet.com/wp-content/uploads/2016/01/Rye-Bread-8.jpg",
    "https://baregomad.dk/wp-content/uploads/2020/06/rugbr%C3%B8d-med-surdej-2.jpg",
    "https://cdn-rdb.arla.com/dagrofa-dk/rugbroed-solsikkefroe-og-oel/809889741.jpeg",
    "https://madensverden.dk/wp-content/uploads/2021/08/hjemmebagt-kernerugbroed.jpg",
  ];

  let img = imgs[Math.floor(Math.random() * imgs.length)];

  onMount(async () => {
    await new Promise((resolve) => randomimg());
  });

  const randomimg = async () => {
    setTimeout(() => {
      img = imgs[Math.floor(Math.random() * imgs.length)];
      randomimg();
    }, 1000);
  };
</script>

<svelte:head>
  <title>THE RYEBREAD MANIFESTO</title>
  <meta
    name="description"
    content="An official declaration on the supremacy of ryebread. Dense, dark, and sovereign — the bread of the strong."
  />
</svelte:head>

<div class="page">
  <!-- Art Deco header ornament -->
  <div class="ornament-top">
    <div class="deco-line"></div>
    <div class="deco-diamond"></div>
    <div class="deco-line"></div>
  </div>

  <header>
    <span class="overline">AN OFFICIAL DECLARATION</span>
    <h1>THE RYEBREAD<br/>MANIFESTO</h1>
    <span class="subtitle">ISSUED IN THE NAME OF THE GRAIN & THE PEOPLE</span>
  </header>

  <div class="ornament">
    <div class="deco-line"></div>
    <div class="deco-diamond"></div>
    <div class="deco-line"></div>
  </div>

  <section class="hero-image">
    <div class="image-frame">
      <picture>
        <img src={img} alt="Ryebread — The Sovereign Loaf" />
      </picture>
    </div>
  </section>

  <section class="decree">
    <div class="decree-number">I.</div>
    <h2>PREAMBLE</h2>
    <p>
      Everyone should eat ryebread, <strong>the best bread in the world</strong>.
      It tastes supreme among all the breads. Roast it and pair it with every
      type of hummus, tzatziki, and other spreads. It is the singular bread.
      It is the only bread. All other bread is merely flour pretending.
    </p>
  </section>

  <section class="decree">
    <div class="decree-number">II.</div>
    <h2>THE TRANSFORMATION</h2>
    <p>
      As you eat ryebread, feel the wonder of the compressed rye and seeds
      envelop your taste buds and grant you new gut microbiota that will help
      you live a better life. A life more satisfied with yourself. A life where
      your family finally loves you. A life where you know yourself. A life&mdash;
    </p>
    <p class="proclamation">OF RYEBREAD.</p>
  </section>

  <div class="ornament">
    <div class="deco-line"></div>
    <div class="deco-diamond"></div>
    <div class="deco-line"></div>
  </div>

  <section class="decree">
    <div class="decree-number">III.</div>
    <h2>ON THE SUPREMACY OF THE LOAF</h2>
    <p>
      The borders of ryebread have long existed north of central Germany. It is
      eaten in every context in the Nordic kingdom and has since its inception
      been the food of <strong>THE STRONG</strong>.
    </p>
  </section>

  <section class="decree">
    <div class="decree-number">IV.</div>
    <h2>HISTORICAL RECORD</h2>
    <p>
      Ryebread originated in the northern regions as staple food for the people
      because of the food insecurity of the Iron Age. Plinius the Elder, a Roman
      historian, wrote about the bread in his <em>Naturalis Historia</em>. He wrote that
      the bread was made from rye and that it was "the bread of the poor". The
      bread was made from rye and barley, and was baked in a clay oven. He also
      wrote that the bread was "a very sorry food and not fit for consumption
      except to avoid starvation".
    </p>
    <p>
      This view has been <strong>mistakenly held</strong> for many years around the world and is
      recently accentuated by the Usonian sphere of influence due to the
      introduction of the "protein bread" &mdash; the bread you will find if you
      google ryebread. The protein bread is horrible and there is nothing short
      of a subjugation of the West Coast that will make this go away.
    </p>
  </section>

  <div class="ornament">
    <div class="deco-line"></div>
    <div class="deco-diamond"></div>
    <div class="deco-line"></div>
  </div>

  <section class="decree">
    <div class="decree-number">V.</div>
    <h2>ARTICLES OF HEALTH</h2>
    <div class="articles">
      <div class="article">
        <span class="article-marker">A.</span>
        <p>Ryebread is high in fiber, which can help to regulate digestion and keep
        you feeling full longer.</p>
      </div>
      <div class="article">
        <span class="article-marker">B.</span>
        <p>Ryebread is a good source of whole grains, which provide essential
        nutrients like vitamins, minerals, and antioxidants.</p>
      </div>
      <div class="article">
        <span class="article-marker">C.</span>
        <p>Ryebread has a lower glycemic index than white bread, meaning it will not
        cause spikes in blood sugar levels.</p>
      </div>
      <div class="article">
        <span class="article-marker">D.</span>
        <p>Ryebread is naturally low in fat and calories, making it a healthy choice
        for those watching their weight.</p>
      </div>
      <div class="article">
        <span class="article-marker">E.</span>
        <p>Ryebread is a good option for people with celiac disease or gluten
        intolerance, as it is naturally gluten-free.</p>
      </div>
    </div>
  </section>

  <section class="action-block">
    <a href="https://nordicexpatshop.com/DKK/schulstad-skovmand-rye-bread" class="cta">
      PROCURE AUTHENTIC BREAD HERE
    </a>
    <span class="note">(NOT AFFILIATED)</span>
  </section>

  <div class="ornament">
    <div class="deco-line"></div>
    <div class="deco-diamond"></div>
    <div class="deco-line"></div>
  </div>

  <section class="decree warning-section">
    <div class="warning-banner">
      <span class="warning-icon">&#9888;</span>
      <h2>OFFICIAL WARNING</h2>
      <span class="warning-icon">&#9888;</span>
    </div>
    <h3>THE FOLLOWING IS NOT RYEBREAD</h3>
    <p>
      Some shops such as Amazon.com and the general Usonian sphere of influence
      will spout nonsense about how the following image is ryebread.
    </p>
    <p class="proclamation">THIS IS NOT RYEBREAD.</p>
    <p>
      It is a sorry excuse and tastes like it. Beware of imposters out there.
    </p>
    <div class="image-frame warning-image">
      <picture>
        <img
          src="https://www.mestemacher-gmbh.com/wp-content/uploads/2018/09/ProteinBread-GB-RGB_800x707px.png"
          alt="NOT RYEBREAD — A fraudulent impostor"
        />
      </picture>
    </div>
  </section>

  <div class="ornament-top">
    <div class="deco-line"></div>
    <div class="deco-diamond"></div>
    <div class="deco-line"></div>
  </div>

  <footer>
    <p class="seal">&#9670; ANNO MMXXVI &#9670;</p>
    <p class="attribution">Drafted by an Artificial Intelligence &amp; a Dane</p>
  </footer>
</div>

<style>
  :global(*) {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  :global(body) {
    font-family: 'JetBrains Mono', monospace;
    background-color: #0a0a0a;
    color: #e8e0d0;
    min-height: 100vh;
  }

  .page {
    max-width: 820px;
    margin: 0 auto;
    padding: 3rem 2rem;
    border-left: 4px solid #c9a84c;
    border-right: 4px solid #c9a84c;
    background-color: #0d0d0d;
    min-height: 100vh;
  }

  /* Header */
  header {
    text-align: center;
    padding: 2rem 0 1.5rem;
  }

  .overline {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.7rem;
    letter-spacing: 0.5em;
    color: #c9a84c;
    display: block;
    margin-bottom: 1.5rem;
    text-transform: uppercase;
  }

  h1 {
    font-family: 'Bebas Neue', sans-serif;
    font-size: clamp(3.5rem, 10vw, 7rem);
    line-height: 0.95;
    color: #ffffff;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    border-top: 6px solid #c9a84c;
    border-bottom: 6px solid #c9a84c;
    padding: 1rem 0;
    margin: 0.5rem 0;
  }

  .subtitle {
    font-family: 'JetBrains Mono', monospace;
    font-size: 0.6rem;
    letter-spacing: 0.4em;
    color: #8a7a5a;
    display: block;
    margin-top: 1rem;
    text-transform: uppercase;
  }

  /* Ornaments */
  .ornament-top, .ornament {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1rem;
    padding: 1.5rem 0;
  }

  .deco-line {
    flex: 1;
    height: 2px;
    background: linear-gradient(90deg, transparent, #c9a84c, transparent);
  }

  .deco-diamond {
    width: 12px;
    height: 12px;
    background-color: #c9a84c;
    transform: rotate(45deg);
    flex-shrink: 0;
  }

  /* Sections */
  .decree {
    padding: 2rem 0;
    border-bottom: 1px solid #1a1a1a;
  }

  .decree-number {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 2.5rem;
    color: #c9a84c;
    letter-spacing: 0.1em;
    margin-bottom: 0.25rem;
  }

  h2 {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 2rem;
    letter-spacing: 0.15em;
    color: #ffffff;
    text-transform: uppercase;
    margin-bottom: 1.25rem;
    padding-bottom: 0.5rem;
    border-bottom: 3px solid #c9a84c;
    display: inline-block;
  }

  h3 {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 1.5rem;
    letter-spacing: 0.1em;
    color: #e8e0d0;
    text-transform: uppercase;
    margin-bottom: 1rem;
    text-align: center;
  }

  p {
    font-family: 'Playfair Display', serif;
    font-size: 1.05rem;
    line-height: 1.8;
    color: #c8c0b0;
    margin-bottom: 1rem;
  }

  strong {
    color: #c9a84c;
    font-weight: 700;
  }

  em {
    color: #d4c8a8;
  }

  .proclamation {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 2.5rem;
    color: #ffffff;
    text-align: center;
    letter-spacing: 0.15em;
    padding: 1rem 0;
    text-transform: uppercase;
  }

  /* Hero image */
  .hero-image {
    padding: 1.5rem 0;
    display: flex;
    justify-content: center;
  }

  .image-frame {
    border: 4px solid #c9a84c;
    padding: 6px;
    background: #0a0a0a;
    display: inline-block;
  }

  .image-frame img {
    display: block;
    width: 100%;
    max-width: 500px;
    height: auto;
    filter: sepia(15%) contrast(1.1);
  }

  /* Articles */
  .articles {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }

  .article {
    display: flex;
    gap: 1rem;
    align-items: baseline;
    padding: 1rem 1.5rem;
    border-left: 3px solid #c9a84c;
    background-color: rgba(201, 168, 76, 0.03);
  }

  .article-marker {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 1.5rem;
    color: #c9a84c;
    flex-shrink: 0;
    letter-spacing: 0.05em;
  }

  .article p {
    margin-bottom: 0;
    font-size: 0.95rem;
  }

  /* CTA */
  .action-block {
    text-align: center;
    padding: 2.5rem 0;
  }

  .cta {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 1.4rem;
    letter-spacing: 0.2em;
    color: #0a0a0a;
    background-color: #c9a84c;
    padding: 1rem 2.5rem;
    text-decoration: none;
    display: inline-block;
    border: none;
    transition: background-color 0.2s, color 0.2s;
  }

  .cta:hover {
    background-color: #e8e0d0;
    color: #0a0a0a;
  }

  .note {
    display: block;
    font-size: 0.6rem;
    letter-spacing: 0.3em;
    color: #5a5040;
    margin-top: 0.75rem;
    text-transform: uppercase;
  }

  /* Warning */
  .warning-section {
    background-color: rgba(180, 40, 40, 0.06);
    border: 2px solid #8b2020;
    padding: 2rem;
    margin: 1rem 0;
  }

  .warning-banner {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1rem;
    margin-bottom: 1rem;
  }

  .warning-banner h2 {
    color: #cc3333;
    border-bottom-color: #cc3333;
    margin-bottom: 0;
  }

  .warning-icon {
    font-size: 1.5rem;
    color: #cc3333;
  }

  .warning-image {
    border-color: #8b2020;
    margin: 1.5rem auto 0;
    display: block;
    text-align: center;
  }

  .warning-image img {
    max-width: 350px;
    filter: sepia(5%) contrast(1.05);
  }

  /* Footer */
  footer {
    text-align: center;
    padding: 2rem 0 1rem;
  }

  .seal {
    font-family: 'Bebas Neue', sans-serif;
    font-size: 1.3rem;
    color: #c9a84c;
    letter-spacing: 0.3em;
    margin-bottom: 0.75rem;
  }

  .attribution {
    font-size: 0.75rem;
    color: #5a5040;
    letter-spacing: 0.15em;
    font-style: italic;
  }

  /* Responsive */
  @media (max-width: 600px) {
    .page {
      padding: 2rem 1rem;
      border-left-width: 2px;
      border-right-width: 2px;
    }

    .article {
      padding: 0.75rem 1rem;
    }

    .cta {
      font-size: 1.1rem;
      padding: 0.75rem 1.5rem;
    }

    .warning-section {
      padding: 1.5rem 1rem;
    }
  }
</style>
