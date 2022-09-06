<template>
    <main>
        <div class="jumbotron">
        </div>
        <div class="container">
            <div class="current">
                <h2>current series</h2>
            </div>
            <WidgetCard :comics="comics" />
            <div class="load">
                load more
            </div>
        </div>
    </main>
</template>

<script>
import WidgetCard from './WidgetCard.vue';
const comics = require('../dc-comics.json');


export default {
    data() {
        return {
            comics
        };
    },
    mounted() {
        console.log(this.comics);
    },
    components: { WidgetCard }
}
</script>

<style lang="scss" scoped>
    
    @import '@/style/variables';

    main {
        background-color: $dark;
        color: white;

        .jumbotron {
            background-image: url('@/assets/jumbotron.jpg');
            background-position: top;
            background-size: cover;
            height: 40vh;
        }
        
        .container {
            padding-top: 3rem;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 2rem;
            position: relative;

            .current {
                text-transform: uppercase;
                position: absolute;
                background-color: $dc-blue;
                height: 3rem;
                top: -1.5rem;
                left: 0;
                display: flex;
                justify-content: center;
                align-items: center;
                padding: 0 1rem;
            }

            .load {
                padding: 1rem 5rem;
                background-color: $dc-blue;
                text-transform: uppercase;
                display: inline-block;
                font-weight: bold;
                cursor: pointer;
            }
        }
    }

</style>