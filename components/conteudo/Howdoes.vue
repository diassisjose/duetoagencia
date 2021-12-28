<template>
    <b-container class="py-5 mt-2" id="howdoes">
        <b-row class="my-5 py-5">
            <b-col align="center">
                <img class="img-h" src="~assets/img/solutions.svg" alt="" width="80%">
            </b-col>
            <b-col md="12" sm="12" lg="6" >
                
                <h2 class="h-header">Receba seu material de acordo com sua demanda.</h2>
                <hr class="hr-due" align="left">
                <p class=" mr-5 pr-md-5">
                    Sua empresa existe no mundo digital, e para manter seus futuros e atuais clientes 
                    ligados no que o seu negócio realiza, é necessário gerar conteúdo que tenha
                    relevância para seu público: seja em imagens, textos, vídeos ou <i>'podcasts' </i>.
                    Visite nossos serviços:
                </p>
                <b-row align="center">
                    <b-col>
                        <b-btn block class="pri-btn btndue" href="/#benefits" >Entenda os benefícios</b-btn>
                    </b-col>
                    
                </b-row>
                
            </b-col>
        </b-row>
        <b-row>
            <b-container class="pb-5">
                <CarDu />
            </b-container>
             
        </b-row>
    </b-container>
</template>

<script>
import CarDu from '~/components/itens/card'
export default {
    components:{
        CarDu
    }
}
</script>