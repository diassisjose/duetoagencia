<template>
    <b-container fluid class="footer-due pt-2">
        <b-container class="px-5">
            <b-row class="pt-5"></b-row>
            <b-row>
                <b-col sm="" md="5" lg="6">
                    <p class="footer-p-due smooth-due">CONTEÚDO PARA REDES SOCIAIS</p>
                    <h3 class="text-light">Planejamento e peças digitais para sua empresa</h3>  
                </b-col>
                <b-col sm="" md="4" lg="3">
                    <p class="footer-p-due text-light">A partir de</p>
                    <b-row class="ml-0">
                        <h3 class="text-light">R$ 300,00</h3>
                        <p class="footer-p-due mt-2"> /mensais</p>
                    </b-row>
                </b-col>
                <b-col sm="" md="3" lg="3">
                    <btnDue/>
                </b-col>
            </b-row>
            <br>
            <hr>
            <b-row class="pt-3"></b-row>
            <b-row>
                <b-col sm="12" md="3" lg="3">
                    <img src="~/assets/img/logo-w-dueto.png" width="150" alt="">
                </b-col>
                <b-col sm="12" md="6" lg="6">
                    <b-nav align="center">
                      <b-nav-item class="footerdue-dec" href="/#howdoes">Como funciona</b-nav-item>
                      <b-nav-item class="footerdue-dec" href="/#solutions">Soluções</b-nav-item>
                      <b-nav-item class="footerdue-dec" href="/#benefits">Benefícios</b-nav-item>
                    </b-nav>
                </b-col>
                <b-col sm="12" md="3" lg="3">
                    <a href="https://www.facebook.com/duetoagencia/"><img class="footer-due-el mx-2" src="~/assets/img/001-facebook.svg" alt="Facebook" width="22"></a>
                    <a href="https://www.instagram.com/duetoagencia/"><img class="footer-due-el mx-2" src="~/assets/img/002-instagram.svg" alt="Instagram" width="22"></a>
                    <a href="https://www.linkedin.com/company/dueto-agencia/"><img class="footer-due-el mx-2" src="~/assets/img/003-linkedin.svg" alt="Linkedin" width="22"></a>
                    <a href="https://www.behance.net/agenciadueto"><img class="footer-due-el mx-2" src="~/assets/img/005-brands-and-logotypes.svg" alt="Behance" width="22"></a>
                    <a href="https://api.whatsapp.com/send?phone=553830151700&text=Vamos%20conversar%20Dueto%3F"><img class="footer-due-el mx-2" src="~/assets/img/004-whatsapp.svg" alt="Whatsapp" width="22"></a>
                </b-col>
            </b-row>
            
        </b-container>
        <b-row class="pb-md-1">
            <b-col class="col-2"></b-col>
            <b-col class="pt-md-1 pb-md-1 footer-brand-text" align="center">
                <span><p><strong><a href="https://agenciadueto.com">Dueto Agência Digital ®</a></strong> - Sua melhor experiência em marketing digital está aqui.</p></span>
            </b-col>
            <b-col class="col-2"></b-col>
        </b-row>
    </b-container>
    
</template>
<script>
import btnDue from '~/components/itens/btnDue'
export default {
    components: {
        btnDue
    }
}
</script>