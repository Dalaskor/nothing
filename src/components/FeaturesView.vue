<template>
<section class="features">
    <features class="features__container">
        <div class="features__card">
            <div class="features__logo">
                <img class="features__img" src="./../assets/img/wallpaper.png" alt="wallpaper">
            </div>
            <p class="features__description">
                “a radical reinterpretation of mobile tech”
            </p>
        </div>
        <div class="features__card">
            <div class="features__logo">
                <img class="featurer__img" src="./../assets/img/T3.png" alt="wallpaper">
            </div>
            <p class="features__description">
                “Nothing Phone (1) is the biggest launch of the year in the smartphone space”
            </p>
        </div>
        <div class="features__card">
            <div class="features__logo">
                <img class="featurer__img" src="./../assets/img/GQ.png" alt="wallpaper">
            </div>
            <p class="features__description">
                “The most hyped tech company in years”
            </p>
        </div>
    </features>
</section>
</template>

<script>
export default {
  name: 'FeaturesView',
};
</script>

<style scoped lang="scss">
.features {
  &__container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 64px;
    padding: 56px 0px;
    @media (max-width: 768.98px) {
      flex-wrap: wrap;
      justify-content: center;
    }
  }
  &__card {
    width: 396.33px;
    display: flex;
    flex-direction: column;
    gap: 24px;
    justify-content: center;
  }
  &__logo {
    max-width: 396.33px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  &__img {
  }
  &__description {
    text-align: center;
  }
}

</style>
