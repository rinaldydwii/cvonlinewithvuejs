<template>
  <div class="content-grid-item">
    <div class="content-grid-item-image">
      <object :data="'./static/assets/interest/'+ value.image +'.svg'" type="image/svg+xml"></object>
    </div>
    <div class="content-grid-item-name">{{ value.name }}</div>
  </div>
</template>

<script>
export default {
  props: ['value'],
  name: 'InterestItem'
}
</script>
