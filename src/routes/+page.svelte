<script>
  import { onMount } from "svelte";

  let poems = [
    `There's nothing quite like a slice of rye,

To start your day off right.

This bread is packed with nutrients,

So you can feel good and fight.

Rye bread is hearty and filling,

The perfect way to fuel your body.

With every bite, you're getting stronger,

And that's a feeling everyone should try.`,
    `Rye bread is so delicious
It's hard to resist
The crust is nice and crispy
And the inside is so soft
It's the perfect bread for sandwiches
Or just to eat on its own

There's nothing quite like a freshly baked loaf
The smell is amazing
And the taste is even better
Rye bread is the best
And I'm not just saying that because I'm biased
It's the perfect combination of flavor and texture
And it's healthy too

So if you're looking for a delicious and nutritious bread
Look no further than rye
It's the perfect choice for any meal
And you won't be disappointed`,
    `The ryebread is a staple in many homes
It's a simple bread, but it's so versatile
You can make a sandwich or toast it for breakfast
It's the perfect accompaniment to a meal

There's nothing quite like a slice of ryebread
It's hearty and filling, and it has a great flavor
Whether you're eating it plain or with toppings
It's always a delicious treat

So if you're looking for a tasty bread
That will leave you feeling satisfied
Reach for the ryebread, and you won't be disappointed`,
    `
The sun is high in the sky,
and the scent of baking bread
wafts through the air.

People are busy in the kitchen,
kneading and shaping the dough,
getting ready to bake.

The loaves go into the oven,
and soon the whole house is filled
with the delicious smell.

Everyone gathers around the table,
eager to taste the freshly baked bread.
It's a tradition in Scandinavia,
enjoyed by young and old alike.

There's nothing quite like a slice of ryebread,
topped with butter and jam.
It's a simple pleasure,
but oh so satisfying.`,
    `In Northern Europe,

ryebread is a staple.

It's hearty and filling,

and perfect for a cold winter's day.

There's nothing quite like

a thick slice of ryebread,

toasted and smeared with butter,

to make your day complete.`,
  ];

  let images = [
    "https://marialottes.dk/wp-content/uploads/2019/01/Rugbr%C3%B8d-med-surdej.jpg",
    "https://nordicfoodliving.com/wp-content/uploads/2015/09/20198183221_eb41aa8508_b.jpg",
    "https://889755.smushcdn.com/2066490/wp-content/uploads/2020/05/IMG_0125-750x926.jpg?lossy=1&strip=1&webp=1",
    "https://dk-spisbedre-production.imgix.net/images/recipes/hjemmebagt-rugbrod-med-hvidtol_14543.jpg?fit=crop&crop=focalpoint&fp-x=0.5&fp-y=0.5&fp-z=1.0w=1200&h=628",
    "https://madensverden.dk/wp-content/uploads/2021/08/hjemmebagt-kernerugbroed.jpg",
    "https://albertestengaard.dk/wp-content/uploads/2020/06/glutenfrit-rugbr%C3%B8d-s%C3%B8d-kartoffel-1.jpg",
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
  <p>
    {poem}
  </p>
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
