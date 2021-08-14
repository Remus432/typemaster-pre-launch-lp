<script>
  import Feature from "./Feature.svelte"

  let features = [];

  (async () => {
    const data = await fetch("./data.json")
    const res = await data.json()
    features = [...res.data]
  })()
</script>

<style>
  .features {
    margin-top: 10rem;
  }

  @media (min-width: 768px) {
    .features {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-gap: 10rem;
      margin-bottom: 7.5rem;
    }
  }

  @media (min-width: 1440px) {
    .features {
      grid-template-columns: repeat(4, 1fr);
      margin-top: 15rem;
      grid-gap: 5rem;
    }
  }
</style>

<section class="features">
  {#each features as feature}
    <Feature image={feature.image} headline={feature.headline} description={feature.description} />
  {/each}
</section>