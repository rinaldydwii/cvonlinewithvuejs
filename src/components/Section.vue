<template>
  <section>
    <div class="title">{{ sectionData.title }}</div>
    <div class="content grid-container">
      <div :class="'content-grid ' + sectionData.class" v-if="sectionData.class === 'education'">
        <item-education v-for="value in sectionData.item" :key="value.id" :value="value"></item-education>
      </div>
      <div :class="'content-grid ' + sectionData.class" v-if="sectionData.class === 'organization'">
        <item-organization v-for="value in sectionData.item" :key="value.id" :value="value"></item-organization>
      </div>
      <div :class="'content-grid ' + sectionData.class" v-if="sectionData.class === 'work'">
        <item-work v-for="value in sectionData.item" :key="value.id" :value="value"></item-work>
      </div>
      <div :class="'content-grid ' + sectionData.class" v-if="sectionData.class === 'skill'">
        <item-skill v-for="value in sectionData.item" :key="value.id" :value="value"></item-skill>
      </div>
      <div :class="'content-grid ' + sectionData.class" v-if="sectionData.class === 'interest'">
        <item-interest v-for="value in sectionData.item" :key="value.id" :value="value"></item-interest>
      </div>
      <div :class="'content-grid ' + sectionData.class" v-if="sectionData.class === 'portfolio'">
        <item-portfolio v-for="value in sectionData.item" :key="value.id" :value="value"></item-portfolio>
      </div>
      <div :class="'content-grid ' + sectionData.class" v-if="sectionData.class === 'social-media'">
        <item-social-media v-for="value in sectionData.item" :key="value.id" :value="value"></item-social-media>
      </div>
    </div>
  </section>
</template>

<script>
import EducationItem from './items/EducationItem.vue'
import OrganizationItem from './items/OrganizationItem.vue'
import WorkItem from './items/WorkItem.vue'
import SkillItem from './items/SkillItem.vue'
import InterestItem from './items/InterestItem.vue'
import PortfolioItem from './items/PortfolioItem.vue'
import SocialMediaItem from './items/SocialMediaItem.vue'

export default {
  props: ['sectionData'],
  name: 'Section',
  components: {
    'item-education': EducationItem,
    'item-organization': OrganizationItem,
    'item-work': WorkItem,
    'item-skill': SkillItem,
    'item-interest': InterestItem,
    'item-portfolio': PortfolioItem,
    'item-social-media': SocialMediaItem
  }
}
</script>
