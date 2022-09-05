<template>
  
  <div class="footer-footer">
    <div class="container">
        <div class="sign-up">
            Sign-up now!
        </div>

        <div class="socials">
            <h3 class="socials-title">
                Follow US
            </h3>

            <div class="icons">
                <ul class="list-wrapper">
                    <li>
                        <a href="#nogo">
                            <img src="@/assets/footer-facebook.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            <img src="@/assets/footer-twitter.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            <img src="@/assets/footer-youtube.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            <img src="@/assets/footer-pinterest.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="#nogo">
                            <img src="@/assets/footer-periscope.png" alt="">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
  </div>

</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

    @import '@/style/variables';
    @import '@/style/mixins';

    .footer-footer {
        background-color: $grey;

        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            text-transform: uppercase;

            .sign-up {
                color: white;
                border: 1px solid $dc-blue;
                padding: 1rem;
                cursor: pointer;
            }

            .socials {
                display: flex;
                gap: 2rem;
                align-items: center;

                .socials-title {
                    color: $dc-blue;
                }

                .icons {
                    .list-wrapper {
                        @include list-wrapper;
                    }
                }
            }
        }
    }

</style>