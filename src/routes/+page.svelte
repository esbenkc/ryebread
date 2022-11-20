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
    everyone should eat ryebread, the best bread in the world. it tastes <strong
      >the best</strong
    > of all the breads. roast it and mix it with every type of hummus, tzatziki,
    and other spreads. it is the best bread in the world.
  </p>
  <p>
    as you eat ryebread, feel the wonder of the compressed rye and seeds envelop
    your taste buds and grant you new gut microbiota that will help you live a
    better life. a life more satisfied with yourself. a life where your family
    finally loves you. a life where you know yourself. a life... <strong
      >of ryebread</strong
    >.
  </p>
  <h2>ryebread is the best bread</h2>
  <p>
    the borders of ryebread have long existed north of central germany. it is
    eaten in every context in the nordic kingdom and has since its inception
    been the food of the <strong>strong</strong>.
  </p>
  <p />
  <h2>history</h2>
  <p>
    ryebread originated in the northern regions as staple food for the people
    because of the food insecurity of the iron age. plinius the elder, a roman
    historian, wrote about the bread in his naturalis historia. he wrote that
    the bread was made from rye and that it was "the bread of the poor". the
    bread was made from rye and barley, and was baked in a clay oven. he also
    wrote that the bread was "a very sorry food and not fit for consumption
    except to avoid starvation".
  </p>
  <p>
    this view has been mistakenly held for many years around the world and is
    recently accentuated by the Usonian sphere of influence due to the
    introduction of the "protein bread", the bread you will find if you google
    ryebread. the protein bread is horrible and there is nothing short of a
    subjugation of the west coast that will make this go away.
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
  <a href="https://nordicexpatshop.com/DKK/schulstad-skovmand-rye-bread"
    ><i>Buy real bread here (not affiliated)</i></a
  >
  <div class="line" />
  <h2>WARNING: this is not ryebread</h2>
  <p>
    Some shops such as Amazon.com and the general Usonian sphere of influence
    will spout nonsence about how the following image is ryebread. <b
      >THIS IS NOT RYEBREAD.</b
    > It is a sorry excuse and tastes like it. Beware of imposters out there.
  </p>
  <picture
    ><img
      src="https://www.mestemacher-gmbh.com/wp-content/uploads/2018/09/ProteinBread-GB-RGB_800x707px.png"
      alt="Not ryebread"
      srcset=""
    /></picture
  >
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
