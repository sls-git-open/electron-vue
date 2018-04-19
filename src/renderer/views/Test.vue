<template>
    <div id="wrapper">

        <main>
            <h1>fdfdfd</h1>
        </main>

    </div>
</template>

<script>
    import * as config from '@/config/';

    export default {
        name: 'Test',
        components: {},
        methods: {},
        mounted() {
            console.log(config);
            this.$http.get(`${config.CodingHost}/api/current_user`, {
                headers: {
                    Authorization: `token ${config.CodingToken}`
                }
            }).then(res => {
                console.log(res);
            }).catch(err => {
                console.log(err);
            });
        },
    }
</script>

<style>

</style>
