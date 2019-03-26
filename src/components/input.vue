<template>
  <p>
    <input type="text" placeholder="入力してください">
    <button @click="onAddClick">追加</button>
    <button @click="onDeleteClick">削除</button>
  </p>
</template>

<script lang="ts">
import { Component, Vue, Watch, Prop, Emit } from "vue-property-decorator";
@Component
export default class Input extends Vue {
  @Prop()
  public addData!: string;

  @Emit()
  public add(data: string) {}

  @Emit()
  public delete() {}

  public onAddClick() {}
  public onDeleteClick() {}
}
</script>

<style>
</style>
