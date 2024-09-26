<template>
    <div>
        <h1>测试文本</h1>
        <div>修改public/app.config.js:showExternalText为<b style="color: orange">true</b>即可看到更多内容！</div>
        <h1 v-show="appConfig.showExternalText">闪亮登场！</h1>
    </div>
</template>

<script lang="ts" setup>
import appConfig from "@/app.config";
</script>

<style lang="scss">
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
    > div {
        font-size: 22px;
    }
}

h1:last-child {
    color: #0000;
    background: linear-gradient(aqua, pink);
    -webkit-background-clip: text;
}
</style>
