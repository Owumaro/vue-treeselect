<template>
  <div :class="`vue-treeselect__${type}-tip`">
    <div class="vue-treeselect__icon-wrapper"><span :class="`vue-treeselect__icon-${icon}`" /></div>
    <span :class="`vue-treeselect__${type}-tip-text`"><slot /></span>
  </div>
</template>

<script>
  export default {
    name: 'vue-treeselect--tip',
    props: {
      type: {
        type: String,
        required: true,
      },
      icon: {
        type: String,
        required: true,
      },
    },
  }
</script>
