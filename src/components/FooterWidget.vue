<template>
    <div class="list-wrapper">

        <ul class="list">

            <li class="list-title">
                <h3>
                    {{ title }}
                </h3>
            </li>

            <li v-for="name,i in widget" :key="i">
                <a href="#nogo">
                    {{ name }}
                </a>
            </li>
        </ul>

    </div>

</template>

<script>
export default {
    props: {
        title: String,
        widget: Array
    }
}
</script>

<style lang="scss" scoped>

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

            li a:hover {
                text-decoration: underline;
            }
        }
    }

</style>