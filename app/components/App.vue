<template>
    <Page>
        <ActionBar title="Welcome to NativeScript-Vue!"/>
        <GridLayout columns="*" rows="*">
            <Label class="main-text" :text="msg" />
        </GridLayout>
    </Page>
</template>

<script lang="ts">
  import {Component} from 'vue-property-decorator';
  import NativeScriptVue from 'nativescript-vue';

  @Component
  export default class App extends NativeScriptVue {
    msg = 'Hello World!';
  }
</script>

<style scoped>
    ActionBar {
        background-color: #53ba82;
        color: #ffffff;
    }

    .main-text {
        color: #4e4e4e;
        vertical-align: center;
        text-align: center;
        font-size: 20;
    }
</style>
