<template>
  
  <header class="container">
    <div class="logo">
        <img src="@/assets/dc-logo.png" alt="DC Logo">
    </div>

    <nav class="main-nav">

        <ul class="nav__list">

            <li class="nav__list__item">
                <a href="#">
                    characters
                </a>
            </li>

            <li class="nav__list__item active">
                <a href="#">
                    comics
                </a>
            </li>

            <li class="nav__list__item">
                <a href="#">
                    movies
                </a>
            </li>

            <li class="nav__list__item">
                <a href="#">
                    tv
                </a>
            </li>

            <li class="nav__list__item">
                <a href="#">
                    games
                </a>
            </li>

            <li class="nav__list__item">
                <a href="#">
                    collectibles
                </a>
            </li>

            <li class="nav__list__item">
                <a href="#">
                    videos
                </a>
            </li>

            <li class="nav__list__item">
                <a href="#">
                    fans
                </a>
            </li>

            <li class="nav__list__item">
                <a href="#">
                    news
                </a>
            </li>

            <li class="nav__list__item">
                <a href="#">
                    shop
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

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .logo {
            height: 100px;
        }

        .main-nav {
            .nav__list{
                display: flex;
                gap: 1.5rem;

                .nav__list__item {
                    text-transform: uppercase;
                    font-weight: bold;
                    font-size: 1rem;
                    
                    &.active, &:hover {
                        color: $dc-blue;
                        position: relative;
                    }
                    
                    &.active:after, &:hover:after{
                        position: absolute;
                        height: 5px;
                        width: 100%;
                        background-color: $dc-blue;
                        left: 0;
                        bottom: calc(-50px + 0.5rem - 2rem);
                        content: '';
                    }
                }
            }
        }
    }

</style>