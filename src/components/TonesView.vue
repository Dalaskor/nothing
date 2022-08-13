<template>
<section class="tones">
    <div class="tones__container">
        <div class="tones__column tones__column_1">
            <div class="tones__image-left">
                <img src="./../assets/img/ear-black.png"
                    alt="Case of white earphones" class="tones__img-left" id="tonesImageLeft">
            </div>
        </div>
        <div class="tones__column tones__column_2">
            <div class="tones__content">
                <div class="tones__body">
                    <h2 class="tones__title">Dark Tones, Brilliant Sound</h2>
                    <p class="tones__description">
                        You already know ear (1) white. Now, get ready
                        for the new ear (1) black edition.
                        It’s moody, smoky and elegant.
                    </p>
                </div>
                <a href="#" class="tones__button btn btn_black">BUY NOW</a>
            </div>
        </div>
        <div class="tones__column tones__column_3">
            <div class="tones__image-right" id="tonesImageRight">
                <img  src="./../assets/img/ear-case-black.png"
                    alt="Case of white earphones" class="tones__img-right">
            </div>
        </div>
    </div>
</section>
</template>

<script>
/* eslint-disable */
export default {
  name: 'TonesView',
};

window.addEventListener('scroll', () => {
  const scrollCount = window.pageYOffset;
  // 976 to 1755
  const minScroll = 976;
  const maxScroll = 1755;
  if (window.innerWidth > 1087.99) {
    if (scrollCount >= minScroll && scrollCount <= maxScroll) {
        const proc = -150+(150 * (scrollCount - minScroll) / (maxScroll - minScroll));
        document.getElementById('tonesImageRight').style.transform = 'translate(' + (0-proc) + '%, ' + 0 + '%) ' +
            'scale(' + (100 - proc) + '%)';
    }
  } else {
    // 3116
    if (scrollCount < 3116) {
        document.getElementById('tonesImageLeft').style.display = 'none';
    } else {
        document.getElementById('tonesImageLeft').style.display = 'inline';
    }
  }
});
</script>

<style scoped lang="scss">
.tones {
  background-color: #fff;
  color: #000;
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
        background-color: #fff;
        position: relative;
        z-index: 11;
        @media (max-width: 1087.99px) {
          grid-column: 1 / 4;
          grid-row: 1;
          height: 100vh;
        }
      }
      &_2 {
        grid-column: 2;
        grid-row: 1;
        background-color: #fff;
        padding: 252px 0px 286px 0px;
        z-index: 999;
        @media (max-width: 1087.99px) {
          grid-column: 1 / 4;
          grid-row: 3;
        }
      }
      &_3 {
        grid-column: 3;
        grid-row: 1;
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 999;
        background-color: #fff;
        @media (max-width: 1087.99px) {
          grid-column: 1 / 4;
          grid-row: 2;
          padding: 50px 0;
        }
      }
  }
  &__image-left {
    display: flex;
    align-items: center;
    justify-content: center;
    top: 0;
    left: 0;
  }
  &__img-left {
    position: fixed;
    z-index: 5;
    top: 25%;
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
    max-width: 368px;
    max-height: 370.42px;
  }
  &__img-right {
    width: 100%;
    height: 100%;
  }
}
</style>
