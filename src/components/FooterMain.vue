<template>
  
  <div class="footer-main">
    <div class="container">

        <div class="col-6">
            <div class="lists-wrapper">

                <div>

                    <ul class="list">

                        <li class="list-title">
                            <h3>
                                dc comics
                            </h3>
                        </li>

                        <li>
                            <a href="#nogo">
                                Characters
                            </a>
                        </li>

                        <li>
                            <a href="#nogo">
                                Comics
                            </a>
                        </li>

                        <li>
                            <a href="#nogo">
                                Movies
                            </a>
                        </li>

                        <li>
                            <a href="#nogo">
                                TV
                            </a>
                        </li>

                        <li>
                            <a href="#nogo">
                                Games
                            </a>
                        </li>

                        <li>
                            <a href="#nogo">
                                Videos
                            </a>
                        </li>

                        <li>
                            <a href="#nogo">
                                News
                            </a>
                        </li>
                    </ul>

                    <ul class="list">

                        <li class="list-title">
                            <h3>
                                shop
                            </h3>
                        </li>

                        <li>
                            <a href="#nogo">
                                Shop DC
                            </a>
                        </li>

                        <li>
                            <a href="#nogo">
                                Shop DC Collectables
                            </a>
                        </li>

                    </ul>

                </div>

                <ul class="list">

                    <li class="list-title">
                        <h3>
                            dc
                        </h3>
                    </li>

                    <li>
                        <a href="#nogo">
                            Terms Of Use
                        </a>
                    </li>

                    <li>
                        <a href="#nogo">
                            Privacy policy (New)
                        </a>
                    </li>

                    <li>
                        <a href="#nogo">
                            Ad Choice
                        </a>
                    </li>

                    <li>
                        <a href="#nogo">
                            Advertising
                        </a>
                    </li>

                    <li>
                        <a href="#nogo">
                            Jobs
                        </a>
                    </li>

                    <li>
                        <a href="#nogo">
                            Subscription
                        </a>
                    </li>

                    <li>
                        <a href="#nogo">
                            Talent Workshops
                        </a>
                    </li>
                    
                    <li>
                        <a href="#nogo">
                            CPSC Certificates
                        </a>
                    </li>
    
                    <li>
                        <a href="#nogo">
                            Rating
                        </a>
                    </li>
    
                    <li>
                        <a href="#nogo">
                            Shop Help
                        </a>

                    </li>
    
                    <li>
                        <a href="#nogo">
                            Contact Us
                        </a>
                    </li>

                </ul>

                <ul class="list">

                    <li class="list-title">
                        <h3>
                            sites
                        </h3>
                    </li>

                    <li>
                        <a href="#nogo">
                            DC
                        </a>
                    </li>
                    
                    <li>
                        <a href="#nogo">
                            MAD Magazine
                        </a>
                    </li>
    
                    <li>
                        <a href="#nogo">
                            DC Kids
                        </a>
                    </li>
    
                    <li>
                        <a href="#nogo">
                            DC Universe
                        </a>

                    </li>
    
                    <li>
                        <a href="#nogo">
                            DC Power Visa
                        </a>
                    </li>

                </ul>

            </div>
        </div>

        <div class="col-6 bg"></div>

    </div>
  </div>

</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

    .footer-main {
        background-image: url('@/assets/footer-bg.jpg');
        background-size: cover;
    
        .container {
            display: flex;
            padding: 0;
            color: #FFF;

            .col-6 {
                flex-basis: 50%;

                &.bg {
                    background-image: url('@/assets/dc-logo-bg.png');
                    background-repeat: no-repeat;
                    background-position: center;
                }

                .lists-wrapper {
                    padding: 2rem 0;
                    display: flex;
                    gap: 2rem;

                    .list {
                        margin-bottom: 1rem;

                        &:first-child {
                        display: flex;
                        flex-direction: column;
                        }

                        h3 {
                            text-transform: uppercase;
                            font-weight: bold;
                            margin-bottom: 1rem;

                        }

                        li:not(.list-title) {
                            line-height: 1.5rem;
                            font-size: 0.75rem;
                            color: #818181;
                        }
                    }
                }
            }
        }
    }
</style>