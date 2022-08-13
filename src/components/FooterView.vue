<template>
<footer class="footer">
    <div class="footer__container">
        <div class="footer__column">
            <h3 class="footer__title">About</h3>
            <ul class="footer__list">
                <li class="footer__list"><a href="#" class="footer__link">About Us</a></li>
                <li class="footer__list"><a href="#" class="footer__link">Comunity</a></li>
                <li class="footer__list"><a href="#" class="footer__link">Newsroom</a></li>
                <li class="footer__list"><a href="#" class="footer__link">Careers</a></li>
                <li class="footer__list"><a href="#" class="footer__link">Contact</a></li>
                <li class="footer__list"><a href="#" class="footer__link">Legal</a></li>
            </ul>
        </div>
        <div class="footer__column">
            <h3 class="footer__title">Products</h3>
            <ul class="footer__list">
                <li class="footer__list"><a href="#" class="footer__link footer__link_sm">
                    phone (1)
                </a></li>
                <li class="footer__list"><a href="#" class="footer__link  footer__link_sm">
                    ear (1)
                </a></li>
            </ul>
        </div>
        <div class="footer__column">
            <h3 class="footer__title">Support</h3>
            <ul class="footer__list">
                <li class="footer__list"><a href="#" class="footer__link">FAQ</a></li>
                <li class="footer__list"><a href="#" class="footer__link">Contact Support</a></li>
                <li class="footer__list"><a href="#" class="footer__link">Service Centers</a></li>
                <li class="footer__list"><a href="#" class="footer__link">E-waste managment</a></li>
            </ul>
        </div>
        <div class="footer__column">
            <h3 class="footer__title">Download the app</h3>
            <ul class="footer__list">
                <li class="footer__list"><a href="#" class="footer__link">Android</a></li>
                <li class="footer__list"><a href="#" class="footer__link">Ios</a></li>
            </ul>
        </div>
        <div class="footer__column">
            <h3 class="footer__title">Newsletter</h3>
            <form action="#" class="footer__form">
                <!-- eslint-disable-next-line -->
                <input type="email" name="email" id="email" class="footer__input" placeholder="Email address">
                <button class="footer__button btn btn_black">Send</button>
            </form>
        </div>
    </div>
</footer>
</template>

<script>
export default {
  name: 'FooterView',
};
</script>

<style scoped lang="scss">
.footer {
    position: relative;
    z-index: 9999;
    background: #D9D9D9;

    &__container {
        display: flex;
        align-items: start;
        justify-content: space-between;
        flex-wrap: wrap;
        gap: 30px;
        padding: 70px 0px;
    }

    &__column {
        display: flex;
        flex-direction: column;
        gap: 32px;
    }

    &__title {
        font-family: 'Dot Matrix';
        font-style: normal;
        font-weight: 400;
        font-size: 24px;
        line-height: 100%;
        text-transform: uppercase;
    }

    &__list {
        display: flex;
        flex-direction: column;
        gap: 16px;
    }

    &__link {
        text-transform: uppercase;
        color: #000000;
        transition: 0.3s;
        &:hover {
            cursor: pointer;
            opacity: 0.7;
        }

        &_sm {
            text-transform: none;
        }
    }

    &__form {
        display: flex;
        align-items: center;
        justify-content: start;
        flex-wrap: wrap;
        gap: 14px;
    }

    &__input {
        width: 265px;
        height: 46px;
        border: 1px solid #000000;
        border-radius: 5px;
        background-color: #D9D9D9;
        padding: 0px 12px;
    }

    &__button {
    }
}
.btn {

    &_black {
    }
}

</style>
