<template>
  <div class="content-grid-item">
    <a :href="value.link">
      <div class="content-grid-item-logo"><img :src="value.logo"/></div>
      <div class="content-grid-item-username">{{ value.username }}</div>
    </a>
  </div>
</template>

<script>
export default {
  props: ['value'],
  name: 'SocialMediaItem'
}
</script>
