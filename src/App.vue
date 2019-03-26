<template>
  <div id="app">
    <p>
      <MyInput @clicked="onMyInputClicked"></MyInput>
    </p>
  </div>
</template>

<script lang="ts">
import { Component, Watch, Vue } from "vue-property-decorator";
import MyInput from "@/components/input.vue";

@Component({
  components: {
    MyInput
  }
})
export default class App extends Vue {}
</script>