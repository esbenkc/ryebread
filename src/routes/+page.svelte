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
  <title>ryebread manifesto</title>
  <meta
    name="description"
    content="Ryebread is a type of bread made with rye flour. It is usually denser and darker than bread made with wheat flour, and has a distinctive, slightly sour taste. Ryebread is popular in many European countries, particularly in Scandinavia and Germany."
  />
</svelte:head>

<section>
  <picture>
    <img src={img} alt="Ryebread" />
  </picture>
  <h1>the ryebread manifesto</h1>
  <p>
    Ryebread makes people happy. There's no denying that a good slice of rye
    bread can make people happy. A nice, hearty rye bread is the perfect
    addition to any meal, and it's a great way to show your loved ones that you
    care.
  </p>
  <h2>ryebread is the best bread in the world</h2>
  <p>
    Ryebread is a type of bread made with rye flour. It is usually denser and
    darker than bread made with wheat flour, and has a distinctive, slightly
    sour taste. Ryebread is popular in many European countries, particularly in
    Scandinavia and Germany. Ryebread philosophically represents all that is
    good about bread. It is simple, honest, and wholesome. It is the bread of
    the people, and it nourishes both body and soul. Compared to white bread,
    ryebread is a nutritional powerhouse, packed with fiber, vitamins, minerals,
    and antioxidants. It is also lower on the glycemic index, meaning it won't
    cause spikes in blood sugar levels. For all these reasons, ryebread is the
    best bread in the world.
  </p>
  <h2>history</h2>
  <p>
    Ryebread has been around for centuries. It was originally developed in
    Europe as a way to use rye flour, which was a cheaper and more readily
    available alternative to wheat flour. Over time, rye bread became a staple
    food in many parts of Europe, particularly in Scandinavia and Germany. It
    has always represented the strength and fortitude of the human spirit, as it
    is a bread that can withstand the harshest of conditions. In recent years,
    ryebread has experienced a resurgence in popularity, as more and more people
    are realizing its nutritional benefits. Today, ryebread is enjoyed by people
    all over the world, and it is sure to remain a staple food for generations
    to come.
  </p>
  <h2>health</h2>

  <ul>
    <li>
      Ryebread is high in fiber, which can help to regulate digestion and keep
      you feeling full longer.
    </li>
    <li>
      Ryebread is a good source of whole grains, which provide essential
      nutrients like vitamins, minerals, and antioxidants.
    </li>
    <li>
      Ryebread has a lower glycemic index than white bread, meaning it won't
      cause spikes in blood sugar levels.
    </li>
    <li>
      Ryebread is naturally low in fat and calories, making it a healthy choice
      for those watching their weight.
    </li>
    <li>
      Ryebread is a good option for people with celiac disease or gluten
      intolerance, as it is naturally gluten-free.
    </li>
  </ul>
  <div class="line" />
  <p><i>Written by an AI and a Dane</i></p>
</section>

<style>
  :global(body) {
    font-family: monospace;
  }

  p,
  li {
    font-size: 1rem;
    line-height: 1.5;
  }

  h2 {
    font-size: 1.25rem;
    margin-top: 2rem;
  }

  h1 {
    font-size: 2rem;
    text-align: left;
  }

  .line {
    width: 100%;
    height: 1px;
    background-color: #000;
    margin: 1rem 0;
  }

  img {
    height: 300px;
  }
</style>
