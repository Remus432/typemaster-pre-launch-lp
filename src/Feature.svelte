<script>
  export let image;
  export let headline;
  export let description;
</script>

<style>
  .features__item {
    margin-bottom: 8rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

  .features__item-icon {
    margin-bottom: 4rem;
  }

  .features__item-headline {
    font-size: 2.4rem;
    font-weight: 900;
    color: var(--dark-blue);
    text-transform: uppercase;
    margin-bottom: 2rem;
    width: 60%;
  }

  .features__item-description {
    line-height: 2.6rem;
    color: var(--grayish-blue);
    font-size: 1.6rem;
    font-weight: 500;
  }

  @media (min-width: 768px) {
    .features__item {
      align-items: flex-start;
      text-align: left;
    }

    .features__item-headline {
      width: 80%;
    }
  }
</style>

<div class="features__item">
  <img src={image} alt="Highly Compatible" class="features__item-icon" />
  <p class="features__item-headline">{headline}</p>
  <p class="features__item-description">{description}</p>
</div>