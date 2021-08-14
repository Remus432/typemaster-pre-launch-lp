<script>
  import Button from "./Button.svelte";
  import gsap from "gsap";
  import { onMount } from "svelte";

  onMount(() => {
    gsap.from(".header__headline", { y: -100, opacity: 0, duration: .8 })
    gsap.from(".header__description", { y: -100, opacity: 0, duration: .8, delay: .2 })
    gsap.from("button", { y: 50, opacity: 0, duration: .8, delay: .2 })
    gsap.from(".header__release", { y: 50, opacity: 0, duration: .8, delay: .4 })
    gsap.from(".header__thumbnail", { y: -50, scale: 1.2, opacity: 0, duration: 1, stagger: .6, delay: .2 })
  })
  
</script>

<style>
  header {
    margin-top: 6rem;
  }

  .header__headline {
    text-transform: uppercase;
    color: var(--dark-blue);
    font-size: 4.8rem;
    line-height: 4.8rem;
  }

  .header__description {
    color: var(--grayish-blue);
    line-height: 2.6rem;
    font-size: 1.6rem;
    margin: 3.5rem 0;
  }

  .header__cta {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .header__release {
    text-transform: uppercase;
    font-weight: 500;
    color: var(--grayish-blue);
    line-height: 2.6rem;
    font-size: 1.6rem;
  }

  .header__thumbnail {
    margin-top: 7rem;
    width: 120%;
  }

  @media (min-width: 768px) {
    header {
      display: flex;
      align-items: center;
    }

    .header__thumbnail {
      width: 478px;
      height: 447px;
      transform: translateX(15%);
    }
  }

  @media (min-width: 1440px) {
    .header__thumbnail {
      width: 540px;
      height: 480px;
      transform: translateX(0);
    }

    .header__description {
      width: 69%;
    }

    .header__cta {
      width: 50%;
    }
  }
</style>

<header>
  <div class="header__text">
    <h1 class="header__headline">Typemaster <br> Keyboard</h1>
    <p class="header__description">Improve your productivity and gaming without breaking the bank. Upgrade to a high quality mechanical typing experience.</p>
    <div class="header__cta">
      <Button bgColor={"#F16718"} color={"#fff"} hoverBgColor={"#FF9B62"}/>
      <p class="header__release">Release on 5/27</p>
    </div>
  </div>
  <img class="header__thumbnail" src="./img/header.png" alt="Typemaster Keyboard Product Showcase"/>
</header> 