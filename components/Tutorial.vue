<template>
  <h1>NUXT App</h1>
</template>
<script>
export default {
  head() {
    return {
      title: 'Nuxt project | Home',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'The frist nuxt project',
        },
      ],
      htmlAttrs: {
        lang: 'es_ES',
      },
    }
  },
}
</script>
<style>
</style>