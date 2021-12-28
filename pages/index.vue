<template>
  <div>
    <Header />
    <Howdoes />
    <SimuladorMod />
    <Solutions />
    <Benefits />
    <Partners /> 
  </div>
</template>
<script>
import Header from '~/components/conteudo/Header'
import Howdoes from '~/components/conteudo/Howdoes'
import SimuladorMod from '~/components/modal/SimuladorMod'
import Solutions from '~/components/conteudo/Solutions'
import Partners from '~/components/conteudo/Partners'
import Footer from '~/components/conteudo/Footer'
import Benefits from '~/components/conteudo/Benefits'
export default {
  components: {
    Header, Howdoes, SimuladorMod, Solutions, Partners,Footer, Benefits
  }
}
</script>
