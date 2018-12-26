<template>
    <div v-if="hasPrevPage()">
        <img alt="Vue logo" src="../assets/logo.png">
    </div>
</template>


<script>
export default {
    methods: {
        hasPrevPage() {
            // console.log("方法一、route.path:", this.$route.path);
            // return this.$route.path == "/";
            // console.log("方法二、router.history.current:", this.$router.history.current["path"]);
            return this.$router.history.current["path"] == "/";
        }
    }
}
</script>