<template>
    <div class="card-container">
        <div class="card" v-for="(comic, i) in comics" :key="i">
            <a href="#nogo">
                <img :src="comic.thumb" :alt="comic.series">
                <h4>{{ comic.series }}</h4>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        comics: Array
    }
}
</script>

<style lang="scss" scoped>

    .card-container {
        display: grid;
        grid-template-columns: repeat(6, 1fr);
        gap: 1.5rem;
        font-size: 1rem;
        font-weight: normal;

        a{

            &:hover h4 {
                text-decoration: underline;
            }

            img {
                aspect-ratio: 1/1;
                object-fit: cover;
                object-position: top;
                margin-bottom: 1rem;
            }
    
            h4 {
                margin-bottom: 2rem;
            }

        }

    }

</style>