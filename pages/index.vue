<template>
  <Presentation :posts="posts" />
</template>

<script>
import Presentation from '~/components/Presentation'
import { getPosts } from '~/api/api'

export default {
  transition: 'page',
  components: { Presentation },
  async asyncData () {
    const posts = await getPosts(4)
    return { posts }
  }
}
</script>
