<template>
    <div id="app">
        <button @click="onHrefTest">测试页面</button>
        <router-view></router-view>
    </div>
</template>

<script>
    export default {
        name: 'sls-git-open-electron-vue',
        methods: {
            onHrefTest() {
                this.$router.push('/test');
            }
        },
        mounted(){
            console.log(this.$electron);
            console.log(this.$http);
        }
    }
</script>

<style>
    /* CSS */
</style>
