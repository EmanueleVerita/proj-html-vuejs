<script>
import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';
import MainAppSecond from './components/MainAppSecond.vue';
import MainAppThird from './components/MainAppThird.vue';
import FooterApp from './components/FooterApp.vue';


  export default {

    data() {
        return {};
    },
    components: { HeaderApp, MainApp, MainAppSecond, MainAppThird, FooterApp }
}
</script>

<template>
 <HeaderApp/>
 <MainApp/>
 <MainAppSecond/>
 <MainAppThird/>
 <FooterApp/>
</template>

<style lang="scss" scoped>

</style>
