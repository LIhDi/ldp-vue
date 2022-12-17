<template>
  <MobilePage v-if="$q.platform.is.mobile"/>
  <DefaultPage v-if="$q.platform.is.desktop"/>
</template>

<script>
import { defineComponent } from 'vue'
import MobilePage from 'components/MobilePage'
import DefaultPage from 'components/DefaultPage'

export default defineComponent({
  name: 'IndexPage',
  components: { MobilePage, DefaultPage }
})
</script>
