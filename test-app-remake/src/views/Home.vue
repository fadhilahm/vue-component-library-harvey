<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App" />
    <sample-component
      heading-text="This is a text component"
      body-text="Made with love by fadhilahm"
    />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import { SampleComponent } from "vue-component-library";

import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src

@Options({
  components: {
    HelloWorld,
    SampleComponent,
  },
})
export default class Home extends Vue {}
</script>
