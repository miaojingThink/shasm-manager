<template>
    <div class="layout">
        <NavHeader/>
        <app-main/>
    </div>
</template>

<script>
    import NavHeader from './NavHeader.vue'
    import AppMain from './AppMain.vue'
    export default {
        components: {
            NavHeader,
            AppMain
        },
        methods: {
            onSelect(name) {
                this.$router.push(name);
            }
        }
    }
</script>

<style scoped>
    .layout {
        border: 1px solid #d7dde4;
    }
</style>
