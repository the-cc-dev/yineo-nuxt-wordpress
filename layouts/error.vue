<template>
  <div class="container">
    <div class="section has-text-centered">
      <h1 class="title is-1" v-if="error.statusCode === 404">Page non trouvée</h1>
      <h1 v-else>Une erreur {{error.statusCode}} s'est produite</h1>
      <nuxt-link class="button primary" to="/">Retourner à Accueil</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  props: ['error'],
  layout: 'blog' // vous pouvez définir une mise en page personnalisée pour la page d'erreur
}
</script>