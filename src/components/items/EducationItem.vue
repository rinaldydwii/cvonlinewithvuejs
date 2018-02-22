<template>
  <div class="content-grid-item">
    <div class="content-grid-item-icon"><i class="icon ion-pin"></i></div>
    <div class="content-grid-item-year">{{ value.year }}</div>
    <div class="content-grid-item-main-content">{{ value.mainContent }}</div>
    <div class="content-grid-item-sub-content">{{ value.subContent }}</div>
  </div>
</template>

<script>
export default {
  props: ['value'],
  name: 'EducationItem'
}
</script>
