<template>
  <div class="content-grid-item">
    <div class="content-grid-item-image"><img :src="value.image"/></div>
    <div class="content-grid-item-name">{{ value.name }}</div>
  </div>
</template>

<script>
export default {
  props: ['value'],
  name: 'InterestItem'
}
</script>
