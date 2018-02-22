<template>
  <div class="content-grid-item">
    <div class="content-grid-item-logo"><img :src="value.icon" /></div>
    <div class="content-grid-item-skill-name">{{ value.name }}</div>
    <div class="content-grid-item-rate">
      <span v-for="n in value.rate" :key="n"><i class="icon ion-android-star"></i></span>
    </div>
  </div>
</template>

<script>
export default {
  props: ['value'],
  name: 'SkillItem'
}
</script>
