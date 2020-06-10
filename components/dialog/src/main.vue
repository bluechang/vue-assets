<template>
  <div class="sky-dialog__wrapper">
    <div class="sky-dialog">
      <div class="sky-dialog__header">
        <span class="sky-dialog__title">{{ title }}</span>
      </div>
      <div class="sky-dialog__body" >
        <slot></slot>
      </div>
      <div class="sky-dialog__footer">
        <slot name="footer"></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SkyDialog',

  props: {
    title: String
  }
}
</script>

<style lang="sass">
  .sky-dialog__wrapper {
    position: fixed;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    overflow: auto;
  }
</style>