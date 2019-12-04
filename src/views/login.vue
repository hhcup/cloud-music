<template>
    <div class='login'>
        <div class="logo">
            <div class="logo-img"></div>
        </div>
    </div>
</template>
<script>
    export default {
        name: 'login',
        data() {
            return {}
        },
        methods: {}
    }
</script>
<style lang='scss' scoped>
     ::v-deep.login{
        position: relative;
        height: 100%;
        width: 100%;
        background-color: #e60012;
        /deep/ .logo{
            position: absolute;
            left: 50%;
            top: 180px;
            transform: translateX(-50%) translateY(-50%);
            width: 100px;
            height: 100px;
            border-radius: 50%;
            background: red url("../assets/icons/logo.png") no-repeat center;
            background-size: 70%;
        }
    }
</style>