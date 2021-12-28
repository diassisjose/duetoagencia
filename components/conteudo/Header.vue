<template>
    <b-container fluid id="home">
        <b-row class="pb-md-5 img-resp-bg due-space ">
            <b-col sm="12" md="1" lg="1">
                
            </b-col>
            <b-col sm="12" md="11" lg="5" class="space-top due-space ">
                <h1 class="space-top header animate-reveal animate-first h1-resp ">
                    Conteúdo digital para sua empresa.
                </h1>
                <p class="p-header mt-4 mb-4 animate-reveal animate-second space-left p-resp">
                    Poste imagens, vídeos, tenha assessoria, planejamento e acesso a ferramentas digitais
                    para encantar seus futuros e atuais clientes.
                </p>
                <b-col>
                    <b-row align="center" class="hide-desktop">
                        <b-col>
                            <b-btn block class="pri-btn btndue" href="/#solutions" >Conheça nossas soluções</b-btn>
                        </b-col>
                    </b-row>
                    <btnDue class="animate-reveal animate-third hide-mobi mr-3 mb-2"/>
                    <b-btn class="pri-btn-inv animate-reveal animate-third hide-mobi" href="#howdoes"><b>Como funciona?</b></b-btn>
                </b-col>
                </b-col>
            <b-col sm="12" md="12" lg="6" >
                <img 
                    class=" hide-mobi animate-reveal animate-first img-resp"  
                    src="~/static/img/headerdue.svg" 
                    fluid alt="Responsive image" 
                    width="85%">
            </b-col>
        </b-row>        
    </b-container>
</template>
<script>
import btnDue from '~/components/itens/btnDue'
export default {
    components:{
        btnDue
    }
}
</script>