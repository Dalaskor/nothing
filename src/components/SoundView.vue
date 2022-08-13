<template>
<section class="sound" id="sectionSound">
    <div class="sound__container">
        <div class="sound__column sound__column_1">
            <div class="sound__image-left" id="soundImageLeft">
                <img src="./../assets/img/ear-case-white.png"
                    alt="Case of white earphones" class="sound__img-left">
            </div>
        </div>
        <div class="sound__column sound__column_2">
            <div class="sound__content">
                <div class="sound__body">
                    <h2 class="sound__title">Sound of Change</h2>
                    <p class="sound__description">
                        The Nothing ear(1). Rawbeauty with precise engineering
                        and state-of-the-art noise cancellation for a pure sound
                        experience.
                    </p>
                </div>
                <a href="#" class="sound__button btn">BUY NOW</a>
            </div>
        </div>
        <div class="sound__column sound__column_3">
            <div class="sound__image-right">
                <img src="./../assets/img/ear-white.png"
                    alt="Case of white earphones" class="sound__img-right">
            </div>
        </div>
    </div>
</section>
</template>

<script>
/* eslint-disable */
export default {
  name: 'SoundView',
};

window.addEventListener('scroll', () => {
  const scrollCount = window.pageYOffset;
  // 230 to 976
  const minScroll = 230;
  const maxScroll = 976;
  if (scrollCount >= minScroll && scrollCount <= maxScroll) {
    const proc = -150+(150 * (scrollCount - minScroll) / (maxScroll - minScroll));
    document.getElementById('soundImageLeft').style.transform = 'translate(' + proc + '%, ' + proc + '%) ' +
        'scale(' + (100 - proc) + '%)';
  }
});
</script>

<style scoped lang="scss">
.sound {
  background-color: #000;
  color: #fff;
  // position: relative;
  z-index: 9999;
  &__container {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
    grid-template-rows: auto;
    grid-auto-flow: column;
  }
  &__column {
      &_1 {
        grid-column: 1;
        grid-row: 1;
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 10;
        background-color: #000;
        @media (max-width: 1087.99px) {
          grid-column: 1 / 4;
          grid-row: 1;
          padding: 50px 0;
        }
      }
      &_2 {
        grid-column: 2;
        grid-row: 1;
        background-color: #000;
        padding: 252px 0px 286px 0px;
        z-index: 10;
        @media (max-width: 1087.99px) {
          grid-column: 1 / 4;
          grid-row: 3;
        }
      }
      &_3 {
        grid-column: 3;
        grid-row: 1;
        background-color: #000;
        position: relative;
        @media (max-width: 1087.99px) {
          grid-column: 1 / 4;
          grid-row: 2;
          height: 100vh;
        }
      }
  }
  &__image-left {
    max-width: 368px;
    max-height: 370.42px;
  }
  &__img-left {
    width: 100%;
    height: 100%;
  }
  &__content {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 40px;
  }
  &__body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 24px;
  }
  &__title {
    font-family: 'Dot Matrix';
    font-style: normal;
    font-weight: 400;
    font-size: 36px;
    line-height: 100%;
    text-transform: uppercase;
    text-align: center;
  }
  &__description {
    font-size: 22px;
    text-align: center;
  }
  &__button {
  }
  &__image-right {
    @media (max-width: 1087.99px) {
      display: flex;
      align-items: center;
      justify-content: center;
      top: 0;
      left: 0;
    }
    
  }
  &__img-right {
    position: fixed;
    z-index: 5;
    top: 25%;
  }
}
</style>
