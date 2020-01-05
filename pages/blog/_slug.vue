<template>
  <div>
    <h1 class="title is-2 section container has-text-centered" v-if="post === undefined">
      Aucun post trouvé pour cet id
    </h1>
    <Post v-if="post" :post="post" />
  </div>
</template>

<script>
import { getPostBySlug } from '~/api/api'
import Post from '~/components/Post'

export default {
  transition: 'page',
  layout: 'post',
  components: { Post },
  async asyncData (params) {
    return {
      post: await getPostBySlug(params.params.slug)
    }
  }
}
</script>
