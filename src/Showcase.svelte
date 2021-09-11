<style>
  .showcase {
    display: flex;
    margin-top: 3rem;
    flex-direction: column;
  }

  .showcase__imgs {
    display: flex;
  }

  .showcase__img {
    height: 193px;
    border-radius: 10px;
  }

  .showcase__square {
      display: none;
    }

  .showcase__img:nth-of-type(1) {
    width: 129px;
    margin-left: -6rem;
  }

  .showcase__img:nth-of-type(2) {
    width: 220px;
    margin-left: 4rem;
  }
  
  .showcase__headline {
    font-size: 3.2rem;
    font-weight: 900;
    color: var(--dark-blue);
    line-height: 3.6rem;
    margin-bottom: 3rem;
    text-transform: uppercase;
  }

  .showcase__description {
    font-size: 1.6rem;
    color: var(--grayish-blue);
    line-height: 2.6rem;
    width: 90%;
  }

  .showcase__text {
    margin-top: 8rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }


  @media (min-width: 768px) {
    .showcase {
      margin-top: 4rem;
    }

    .showcase__img:nth-of-type(1) {
      width: 214px;
      height: 320px;
      margin-left: 0;
    }

    .showcase__img:nth-of-type(2) {
      width: 445px;
      height: 320px;
      margin-left: 3.5rem;
    }

    .showcase__text {
      flex-direction: row;
      text-align: left;
      justify-content: space-between;
      align-items: center;
    }

    .showcase__description {
      width: 60%;
    }

    .showcase__headline {
      margin-bottom: 0;
    }
  }

  @media (min-width: 1440px) {
    .showcase {
      flex-direction: row;
      align-items: center;
    }

    .showcase__imgs {
      display: flex;
    }

    .showcase__img:nth-of-type(1) {
      width: 255px;
      height: 480px;
      margin-right: 2.5rem;
    }

    .showcase__img:nth-of-type(2) {
      width: 445px;
      height: 480px;
      margin-left: 0;
    }

    .showcase__text {
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-start;
      margin: 0 15rem;
    }

    .showcase__description {
      margin-top: 2rem;
      width: 120%
    }

    .showcase__square {
      display: inline-block;
      position: absolute;
      left: 0;
      align-self: flex-end;
      transform: rotateY(-180deg);
    }
  }
</style>

<section class="showcase">
  <img class="showcase__square" src="./img/bgSquare.svg" alt="Gray Square Graphic Asset"/>
  <div class="showcase__imgs">
    <img class="showcase__img" src="./img/desktop-red.png" alt="Desktop With Red Overlay"/>
    <img class="showcase__img" src="./img/desktop.png" alt="Desktop"/>
  </div>
  <div class="showcase__text">
    <h2 class="showcase__headline">Mechanical <br> Wireless <br> Keyboard</h2>
    <p class="showcase__description">The Typemaster keyboard boasts top-notch build and practical design. It offers a wide variety of switches and keycaps, along with reliable wireless connectivity.</p>
  </div>
</section>