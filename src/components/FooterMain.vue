<template>
  
  <div class="footer-main">
    <div class="container">
        <div>
            <FooterWidget :title="titles[0]" :widget="widgets[0]" />
            <FooterWidget :title="titles[1]" :widget="widgets[1]" />
        </div>
        <FooterWidget :title="titles[2]" :widget="widgets[2]" />
        <FooterWidget :title="titles[3]" :widget="widgets[3]" />
    </div>
  </div>

</template>

<script>

    import widgets from './FooterWidgets';
    import FooterWidget from './FooterWidget.vue';

    export default {
    data() {
        return {
            widgets,
            titles: ['dc comics', 'shop', 'dc', 'sites']
        };
    },
    components: { FooterWidget }
}
</script>

<style lang="scss" scoped>

    .footer-main {
        background-image: url('@/assets/footer-bg.jpg');
        background-size: cover;
    
        .container {
            display: flex;
            padding: 2rem 0;
            color: #FFF;
            background-image: url('@/assets/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: center right;
            gap: 2rem;
        }
    }
</style>