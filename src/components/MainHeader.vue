<template>
  
  <header class="container">
    <div class="logo">
        <img src="@/assets/dc-logo.png" alt="DC Logo">
    </div>

    <nav class="main-nav">

        <ul class="nav__list">

            <li v-for="(widget, i) in widgets" :key="i" :class="[widget.active ? 'active' : '', 'nav__list__item']">
                <a href="#">
                    {{ widget.title }}
                </a>
            </li>
        </ul>

    </nav>
  </header>

</template>

<script>
    import widgets from './HeaderWidgets'

    export default {
        data() {
            return {
                widgets
            }
        }
    }
</script>

<style lang="scss" scoped>

    @import '@/style/variables';
    @import '@/style/mixins';

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .logo {
            height: 100px;
        }

        .main-nav {
            .nav__list{
                @include list-wrapper;
                display: none;

                .nav__list__item {
                    @include list-items;
                    
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

    @media (min-width: 1024px) {
        .nav__list {
            display: flex !important;
        }
    }

</style>