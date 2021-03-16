<template>
  <div class="input">
    <div class="input_head" v-if="label">
      <span>{{ label }}</span>
    </div>
    <input type="text" />
  </div>
</template>

<script lang="ts">
export default {
  props: {
    label: {
      type: String || Number,
      required: true,
      default: ""
    }
  }
};
</script>

<style lang="scss" scoped>
.input {
  width: 100%;
  margin-bottom: rem($gap * 2);
}
</style>
