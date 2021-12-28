<template>
  <div>
    <NavDue />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import NavDue from '~/components/nav/navDue'
import Footer from '~/components/conteudo/Footer'
export default {
  components: {
    NavDue, Footer
  }
}
</script>