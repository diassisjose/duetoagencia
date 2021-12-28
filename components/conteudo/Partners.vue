<template>
    <b-container class="pt-2 pb-5 mb-5">
        <b-row>
            <b-col class="due-space" align="center">
                <h2 class="h-header mb-2">Clientes e Parceiros</h2>
                <hr class="hr-due" align="center">
                <div class="">
                    <carousel 
                        :autoplay="true" 
                        :nav="false"
                        :items="6"
                        :margin="6"
                        :autoplayTimeout="1500"
                        :dots="false"
                        :responsive="{0:{items:2,nav:false},720:{items:3,nav:false},1300:{items:6,nav:false}}"
                        >
                            <b-img v-for="(logo, logos) in logos" :src="'/img/logos/'+logo.clients+'.svg'" :key="logos" class="owl-mobi" :alt="logo.alt"></b-img>
                    </carousel>
                </div>
            </b-col>
           
        </b-row>
    </b-container>
</template>
<script>
export default {
    data() {
        return{
            logos: [
                {
                    clients: 'logo1',
                    alt: 'Ventura Makers - Inovação e Treinamentos',
                },
                {
                    clients: 'logo2',
                    alt: 'Pão de Mel - Supermercado e Padaria'
                },
                {
                    clients: 'logo3',
                    alt: 'Cordeiro Atacarejo'
                },
                {
                    clients: 'logo4',
                    alt: 'Inovar Uniformes'
                },
                {
                    clients: 'logo5',
                    alt: 'Oba Burger - Hamburgeria'
                },
                {
                    clients: 'logo6',
                    alt: 'Bessa Treinamentos'
                },
                {
                    clients: 'logo7',
                    alt: 'JJ Cursos e Treinamentos'
                },
                {
                    clients: 'logo8',
                    alt: 'A3 Studio'
                },
                {
                    clients: 'logo9',
                    alt: 'Miramotors Hyundai'
                },
                {
                    clients: 'logo10',
                    alt: 'Mota Engenharia'
                },
                {
                    clients: 'logo11',
                    alt: 'Drogaria Minas Brasil'
                },
                {
                    clients: 'logo12',
                    alt: 'Legal Cap - Título de Capitalização'
                },
                {
                    clients: 'logo13',
                    alt: 'Proximal Engenharia e Treinamentos'
                },
                {
                    clients: 'logo14',
                    alt: 'Interagir Psicologia'
                },
                {
                    clients: 'logo15',
                    alt: 'Bianca Nunes - Makeup Artist'
                },
                {
                    clients: 'logo16',
                    alt: 'Valdivina Instituto de Beleza'
                },
                {
                    clients: 'logo17',
                    alt: 'Usiara - Usinagem em Contagem'
                },
                {
                    clients: 'logo18',
                    alt: 'Ramones Seguros'
                },
                {
                    clients: 'logo19',
                    alt: 'Prefeitura de Mesquita - RJ'
                },
                {
                    clients: 'logo20',
                    alt: 'Felipe Quadros - Web Developer'
                },
                {
                    clients: 'logo21',
                    alt: 'Hospital Dilson Godinho'
                },
                {
                    clients: 'logo22',
                    alt: 'Extra Energy - Eletricidade e Iluminação Pública'
                },
                {
                    clients: 'logo23',
                    alt: 'Distrinorte Distribuidora'
                },
                {
                    clients: 'logo24',
                    alt: 'Colégio Berlaar Imaculada Conceição'
                },
                {
                    clients: 'logo25',
                    alt: 'SR2 Sistemas'
                },
                {
                    clients: 'logo26',
                    alt: 'INFOMAX - Tecnologia ao seu alcance'
                },
                {
                    clients: 'logo27',
                    alt: 'Exitus Consultoria Financeira'
                },
                {
                    clients: 'logo28',
                    alt: 'O Chefão Pub'
                },
                {
                    clients: 'logo29',
                    alt: 'DX3 Tecnologia'
                },
                {
                    clients: 'logo30',
                    alt: 'Dito Callado Fotografia'
                },
                {
                    clients: 'logo31',
                    alt: 'Revista C&R'
                }
            ],
        }
    }
}
</script>


