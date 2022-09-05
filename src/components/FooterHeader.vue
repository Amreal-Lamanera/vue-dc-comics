<template>
  
    <header>
        <nav class="container">

            <ul class="footer-list">
                <li class="footer__list__item">
                    <a href="#nogo">
                        <img src="@/assets/buy-comics-digital-comics.png" alt="">
                        <span>
                            digital comics
                        </span>
                    </a>
                </li>

                <li class="footer__list__item">
                    <a href="#nogo">
                        <img src="@/assets/buy-comics-merchandise.png" alt="">
                        <span>
                            dc merchandise
                        </span>
                    </a>
                </li>

                <li class="footer__list__item">
                    <a href="#nogo">
                        <img src="@/assets/buy-comics-subscriptions.png" alt="">
                        <span>
                            subscription
                        </span>
                    </a>
                </li>

                <li class="footer__list__item">
                    <a href="#nogo">
                        <img src="@/assets/buy-comics-shop-locator.png" alt="">
                        <span>
                            comic shop locator
                        </span>
                    </a>
                </li>

                <li class="footer__list__item">
                    <a href="#nogo">
                        <img src="@/assets/buy-dc-power-visa.svg" alt="">
                        <span>
                            dc power visa
                        </span>
                    </a>
                </li>
            </ul>

        </nav>
    </header>

</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

    @import '@/style/variables';
    @import '@/style/mixins';

    header {
        background-color: $dc-blue;
    
    .container {
        color: #FFF;
        padding: 3rem 1rem;

        .footer-list {
            @include list-wrapper;

            .footer__list__item {
                @include list-items;

                a {
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    gap: 1rem;

                    img {
                        height: 50px;
                    }
                }

            }

        }
    }
}

</style>