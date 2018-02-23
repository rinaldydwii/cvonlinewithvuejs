<template>
  <section>
    <div class="title">{{ sectionData.title }}</div>
    <div class="content">
      <div class="content-item-birth">{{ sectionData.birth }}</div>
      <div class="content-item-address">{{ sectionData.address1 }}</div>
      <div class="content-item-address">{{ sectionData.address2 }}</div>
    </div>
    <hr />
  </section>
</template>

<script>
export default {
  props: ['sectionData'],
  name: 'Profile'
}
</script>
