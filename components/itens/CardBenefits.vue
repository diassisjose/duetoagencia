<template>
    <b-container>
            <b-card-group deck class="my-md-3 mb-sm-0">
                <b-card>
                    <b-row>
                        <b-col md="2" class="mx-2 mb-4 mr-5">
                            <img class="mobi-card-ben pulse" src="~/static/img/socialmedia-due.svg" alt="..." width="110">
                        </b-col>
                        <b-col>
                            <h3 class="h-blurb">Imagens e Vídeos<br> para Redes Sociais</h3>
                            <p class="footer-p-due part-due">Pacotes a partir de</p>
                            <b-row class="ml-0">
                                <h3 class="part-due">R$ 300,00</h3>
                                <p class="footer-p-due mt-2"> /mensais</p>
                            </b-row>
                            <b-button class="btn-sm" v-b-modal.modal-1>{{ add }}</b-button>
                            <p class="p-card">
                                Vamos desenvolver um pacote de imagens para Redes Sociais 
                                baseado na estratégia da sua empresa para a captação e 
                                comunicação com seu público alvo.
                            </p>
                            <a :href="list+'marketing-de-conteudo'" class="p-card-due-small">    
                                {{ btnlink }}
                                <img class="ml-2 " src="~/assets/img/right-arrow.svg" width="15px" />
                            </a>
                        </b-col>
                    </b-row>
                </b-card>
                <b-card>
                    <b-row>
                        <b-col md="2" class="mx-2 mb-4 mr-5">
                            <img class="mobi-card-ben pulse" src="~/static/img/smmanager-due.svg" alt="..." width="110">
                        </b-col>
                        <b-col>
                            <h3 class="h-blurb">Plano de Comunicação <br>nas Redes Sociais</h3>
                            <p class="footer-p-due part-due">Pacotes a partir de</p>
                            <b-row class="ml-0">
                                <h3 class="part-due">R$ 360,00</h3>
                                <p class="footer-p-due mt-2"> /mensais</p>
                            </b-row>
                            <b-button class="btn-sm" v-b-modal.modal-1>{{ add }}</b-button>
                            <p class="p-card">
                                Ainda não tem uma equipe para gerenciar, entender, planejar executar 
                                suas demandas de comunicação nas Redes Sociais? Pode contar com a nossa!    
                            </p>
                            <a :href="list+'social-media'" class="p-card-due-small">    
                                {{ btnlink }}
                                <img class="ml-2 " src="~/assets/img/right-arrow.svg" width="15px" />
                            </a>
                        </b-col>
                    </b-row>
                </b-card>
            </b-card-group>
            <b-card-group class="my-md-3 mb-sm-0" deck>
                <b-card>
                    <b-row>
                        <b-col md="2" class="mx-2 mb-4 mr-5">
                            <img class="mobi-card-ben pulse" src="~/static/img/targetads-due.svg" alt="..." width="110">
                        </b-col>
                        <b-col>
                            <h3 class="h-blurb">Anúncios Digitais: <br>do Facebook ao Google</h3>
                            <p class="footer-p-due part-due">Pacotes a partir de</p>
                            <b-row class="ml-0">
                                <h3 class="part-due">R$ 430,00</h3>
                                <p class="footer-p-due mt-2"> /mensais</p>
                            </b-row>
                            <b-button class="btn-sm" v-b-modal.modal-1>{{ add }}</b-button>
                            <p class="p-card">
                                De acordo com suas metas e prazos, criamos anúncios para captar e 
                                converter as ações do seu público alvo, gerando performance e resultados.
                            </p>
                            <a :href="list+'links-patrocinados'" class="p-card-due-small">    
                                {{ btnlink }}
                                <img class="ml-2 " src="~/assets/img/right-arrow.svg" width="15px" />
                            </a>
                        </b-col>
                    </b-row>
                </b-card>
                <b-card>
                    <b-row>
                        <b-col md="2" class="mx-2 mb-4 mr-5">
                            <img class="mobi-card-ben pulse" src="~/static/img/inboundmkt-due.svg" alt="..." width="110">
                        </b-col>
                        <b-col>
                            <h3 class="h-blurb">Encantamento com <br>Inbound Marketing</h3>
                            <p class="footer-p-due part-due">Pacotes a partir de</p>
                            <b-row class="ml-0">
                                <h3 class="part-due">R$ 720,00</h3>
                                <p class="footer-p-due mt-2"> /mensais</p>
                            </b-row>
                            <b-button class="btn-sm" v-b-modal.modal-1>{{ add }}</b-button>
                            <p class="p-card">
                                A palavra-chave do Marketing Digital é Estratégia. E para você que deseja encantar
                                seus clientes e fidelizar, o Inbound Marketing é o melhor caminho. Solicite seu orçamento.
                            </p>
                            <a :href="list+'inbound-marketing'" class="p-card-due-small">    
                                {{ btnlink }}
                                <img class="ml-2 " src="~/assets/img/right-arrow.svg" width="15px" />
                            </a>
                        </b-col>
                    </b-row>
                </b-card>
            </b-card-group> 
            <b-card-group class="my-md-3 mb-sm-0" deck>
                <b-card>
                    <b-row>
                        <b-col md="2" class="mx-2 mb-4 mr-5">
                            <img class="mobi-card-ben pulse" src="~/static/img/emailmkt-due.svg" alt="..." width="110">
                        </b-col>
                        <b-col>
                            <h3 class="h-blurb">Seu relacionamento<br> com Email Marketing</h3>
                            <p class="footer-p-due part-due">Pacotes a partir de</p>
                            <b-row class="ml-0">
                                <h3 class="part-due">R$ 620,00</h3>
                                <p class="footer-p-due mt-2"> /mensais</p>
                            </b-row>
                            <b-button class="btn-sm" v-b-modal.modal-1>{{ add }}</b-button>
                            <p class="p-card">
                                Converse com seu cliente, dê dicas, orientações, presentes e conquiste
                                sua confiança de forma cíclica: seja aquela empresa que contribui, não a que envia "spam"!
                            </p>
                            <a :href="list+'email-marketing'" class="p-card-due-small">    
                                {{ btnlink }}
                                <img class="ml-2 " src="~/assets/img/right-arrow.svg" width="15px" />
                            </a>
                        </b-col>
                    </b-row>
                </b-card>
                <b-card>
                    <b-row>
                        <b-col md="2" class="mx-2 mb-4 mr-5">
                            <img class="mobi-card-ben pulse" src="~/static/img/devweb-due.svg" alt="..." width="110">
                        </b-col>
                        <b-col>
                            <h3 class="h-blurb">Do Site ao Aplicativo: <br>sua empresa merece evoluir</h3>
                            <p class="footer-p-due part-due">Pacotes a partir de</p>
                            <b-row class="ml-0">
                                <h3 class="part-due">R$ 540,00</h3>
                                <p class="footer-p-due mt-2"> /mensais</p>
                            </b-row>
                            <b-button class="btn-sm" v-b-modal.modal-1>{{ add }}</b-button>
                            <p class="p-card">
                                Eles são a sua empresa aberta 24h, vendendo para seu público ou captando 
                                futuros clientes: tenha a tecnologia necessária para melhorar suas vendas!
                            </p>
                            <a :href="list+'site-e-blog'" class="p-card-due-small">    
                                {{ btnlink }}
                                <img class="ml-2 " src="~/assets/img/right-arrow.svg" width="15px" />
                            </a>
                        </b-col>
                    </b-row>
                </b-card>
            </b-card-group> 
    </b-container>
</template>
<script>
export default {
    data() {
        return{
            add:`ORÇAMENTO`,
            btnlink: `Mais informações`,
            list: "https://agenciadueto.com/",
            actionbtn: `v-b-modal.modal-1`
        }
    }
}
</script>