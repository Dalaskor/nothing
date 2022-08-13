<template>
<section class="about">
    <div class="about__container">
        <h2 class="about__title">About Us</h2>
        <p class="about__description">
            We’re a London-based tech company on
            a mission to remove barriers between
            people and technology. Lets make tech
            not so boring.
        </p>
    </div>
</section>
</template>

<script>
export default {
  name: 'AboutView',
};
</script>

<style scoped lang="scss">
.about {
    position: relative;
    z-index: 9999;
    background-color: #EAEDEA;
    &__container {
        padding: 100px 0px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        max-width: 500px;
        gap: 30px;
    }
    &__title {
        font-family: 'Dot Matrix';
        font-style: normal;
        font-weight: 400;
        font-size: 36px;
        line-height: 100%;
        text-transform: uppercase;
    }
    &__description {
        font-size: 22px;
        text-align: center;
    }
}
</style>
