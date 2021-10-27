<template>
  <div>
    <h1>Hello I'm consuming the component library</h1>
    <sample-component
      heading-text="This is a text component"
      body-text="Made with love by Fadhilahm"
    />
  </div>
</template>

<script>
import { Component, Vue } from "vue-property-decorator";

import { SampleComponent } from "vue-component-library-harvey";

@Component({
  SampleComponent,
})
export default class Test extends Vue {}
</script>

<style></style>
