<template>
    <b-row>
        <b-card-group deck>
            <b-card class="card-due card-due-mobi m-3">
                <img class="mx-4 pt-4 mb-4" src="~/assets/img/001-process.svg" alt="" width="40">
                <b-card-title class="mx-4 h-card-due">Conheça as soluções que projetamos</b-card-title>
                <b-col cols="4"><hr class="mx-2"></b-col>
                <p class="mx-4 p-card-due ">
                    Entenda cada uma das facilidades que desenvolvemos para sua empresa: assim podemos 
                    criar um orçamento personalizado e de acordo com seu bolso.
                    <br>
                    <a href="/#solutions" class="p-card-due-small">
                        <i class="icon ion-md-cog" style="font-size:16px;"></i>
                        Conheça nossas soluções
                    </a>
                </p>
            </b-card>
            <b-card class="card-due card-due-mobi m-3">
                <img class="mx-4 pt-4 mb-4" src="~/assets/img/002-yes.svg" alt="" width="40">
                <b-card-title class="mx-4 h-card-due">Selecione quais se adequam a sua necessidade</b-card-title>
                <b-col cols="4"><hr class="mx-2"></b-col>
                <p class="mx-4 p-card-due">
                    Quando decidir quais serviços sua empresa tem prioridade, necessidade, ou que 
                    podemos executar para melhorar o tempo de trabalho da sua equipe, "marque" cada um no <b>Orçamento.</b>
                </p>
            </b-card>
            <b-card class="card-due card-due-mobi m-3" align="center">
                <img class="mx-4 pt-5 mb-4 mt-4" src="~/assets/img/003-review.svg" alt="" width="70">
                <b-card-title class="mx-4 h-card-due">Nossa equipe entrará em contato!</b-card-title>
                <btnDue class="mt-3" align="center"/>
            </b-card>
        </b-card-group>
    </b-row>
</template>
<script>
import btnDue from '~/components/itens/btnDue'
export default {
    components:{
        btnDue
    }
}
</script>