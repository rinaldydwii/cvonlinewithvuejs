<template>
  <div>
    <app-header></app-header>
    <app-main></app-main>
  </div>
</template>

<script>
import Header from './Header'
import Main from './Main'

export default {
  name: 'HomePage',
  components: {
    'app-header': Header,
    'app-main': Main
  }
}
</script>
