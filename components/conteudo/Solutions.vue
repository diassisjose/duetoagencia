<template>
    <b-container fluid class="section-space bg-benefits" id="solutions">
        <b-container>
            <b-row>
                <b-col sm md lg></b-col>
                <b-col sm md="8" lgclass="mt-md-5 pt-3" align="center">
                    <h2 class="h-header mx-md-2">
                        Selecione quais facilidades gostaria de receber em sua proposta.</h2>
                    <hr class="hr-due" align="center">
                    <!-- <p>
                        Sua empresa existe no mundo digital, e para manter seus futuros e atuais clientes 
                        ligados no que o seu negócio realiza, é necessário gerar conteúdo que tenha
                        relevância para seu público: seja em imagens, textos, vídeos ou <i>'podcasts' </i>.
                        Visite nossos serviços:
                    </p> -->
                </b-col>
                <b-col sm md lg></b-col>
            </b-row>
            <b-row class="mt-2 due-space">
                <CardDue />
            </b-row>
        </b-container>
    </b-container>
</template>

<script>
import CardDue from '~/components/itens/CardBenefits'
export default {
    components: {
        CardDue
    }
}
</script>