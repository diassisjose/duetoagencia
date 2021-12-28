<template>

        <b-modal class="modaldue" hide-footer id="modal-1" size="xl">
            <b-row>
                <b-col class="modal-title" >
                    <h3 class="h-modal">Tenha seu plano sob demanda</h3>
                    <h5 class="h5-modal">Escolha as opções que deseja receber </h5>
                </b-col>
            </b-row>
            <b-row>
                <b-form name="form-leads" action="POST" method="post" data-netlify="true" data-netlify-honeypot="bot-field">
                <input type="hidden" name="form-name" value="form-leads" /> 
                    <b-col>
                        <b-col cols="8">
                            <b-row>
                                <b-col cols="2" class="switchdeact mx-1 my-1 " v-on:click="registration.checkedPlan1 = !registration.checkedPlan1" :class="{checked: registration.checkedPlan1}">
                                    <h4 class="h-switch">Imagens para Redes Sociais</h4>
                                    <p class="p-switch">Tenha conteúdos criados diretamente para seu público</p>
                                    <b-col align="right" class="footer-switch">
                                        <input 
                                            class="footer-switch" 
                                            type="checkbox" 
                                            value="socialMedia" 
                                            name="socialMedia" 
                                            id="socialMedia"
                                            v-model="registration.checkedPlan1"
                                            >
                                    </b-col>
                                </b-col>
                                <b-col cols="2" class="switchdeact mx-1 my-1 " v-on:click="registration.checkedPlan2 = !registration.checkedPlan2" :class="{checked: registration.checkedPlan2}">
                                    <h4 class="h-switch">Conteúdo para Blog Corporativo</h4>
                                    <p class="p-switch">Tenha conteúdos criados diretamente para seu público</p>
                                    <b-col align="right" class="footer-switch">
                                        <input 
                                            class="footer-switch" 
                                            type="checkbox" 
                                            value="contentMkt" 
                                            name="contentMkt"
                                            id="contentMkt"
                                            v-model="registration.checkedPlan2"
                                        >
                                    </b-col>
                                </b-col>
                                <b-col cols="2" class="switchdeact mx-1 my-1 " v-on:click="registration.checkedPlan3 = !registration.checkedPlan3" :class="{checked: registration.checkedPlan3}">
                                    <h4 class="h-switch">Publicidade Paga</h4>
                                    <p class="p-switch">Tenha conteúdos criados diretamente para seu público</p>
                                    <b-col align="right" class="footer-switch">
                                        <input 
                                            class="footer-switch" 
                                            type="checkbox" 
                                            value="socialAds" 
                                            name="socialAds" 
                                            id="socialAds" 
                                            v-model="registration.checkedPlan3"
                                        >
                                    </b-col>
                                </b-col>
                                <b-col cols="2" class="switchdeact mx-1 my-1 " v-on:click="registration.checkedPlan4 = !registration.checkedPlan4" :class="{checked: registration.checkedPlan4}">
                                    <h4 class="h-switch">Email Marketing</h4>
                                    <p class="p-switch">Tenha conteúdos criados diretamente para seu público</p>
                                    <b-col align="right" class="footer-switch">
                                        <input 
                                            class="footer-switch" 
                                            type="checkbox" 
                                            value="emailMkt" 
                                            name="emailMkt" 
                                            id="emailMkt" 
                                            v-model="registration.checkedPlan4"
                                        >
                                    </b-col>
                                </b-col>
                                <b-col cols="2" class="switchdeact mx-1 my-1 " v-on:click="registration.checkedPlan5 = !registration.checkedPlan5" :class="{checked: registration.checkedPlan5}">
                                    <h4 class="h-switch">Inbound Marketing</h4>
                                    <p class="p-switch">Tenha conteúdos criados diretamente para seu público</p>
                                    <b-col align="right" class="footer-switch">
                                        <input 
                                            class="footer-switch" 
                                            type="checkbox" 
                                            value="inboundMkt" 
                                            name="inboundMkt" 
                                            id="inboundMkt" 
                                            v-model="registration.checkedPlan5"
                                        >
                                    </b-col>
                                </b-col>
                                <b-col cols="2" class="switchdeact mx-1 my-1 " v-on:click="registration.checkedPlan6 = !registration.checkedPlan6" :class="{checked: registration.checkedPlan6}">
                                    <h4 class="h-switch">Desenvolvimento Web</h4>
                                    <p class="p-switch">Tenha conteúdos criados diretamente para seu público</p>
                                    <b-col align="right" class="footer-switch">
                                        <input 
                                            class="footer-switch" 
                                            type="checkbox" 
                                            value="webDev" 
                                            name="webDev" 
                                            id="webDev" 
                                            v-model="registration.checkedPlan6"
                                        >
                                    </b-col>
                                </b-col>
                            </b-row>
                        </b-col>
                        <b-col cols="3">
                                <!-- <b-row>
                                    <b-col align="right" class="mt-3">
                                        <b-button class="sec-btn ml-md-3" @click.prevent="next()" >Texto Botão</b-button>
                                    </b-col>
                                </b-row> -->
                            <b-row class="bg-form">
                                <b-col md="6">
                                        <p class="label-input-due mt-3">Seu nome</p>
                                        <b-form-input 
                                            class="form-due" 
                                            v-model="registration.name" 
                                            id="name" 
                                            name="name" 
                                            placeholder="Seu nome"
                                            required
                                            >
                                        </b-form-input>
                                </b-col>
                                <b-col md="6">
                                        <p class="label-input-due mt-3">Seu nome</p>
                                        <b-form-input 
                                            class="form-due" 
                                            v-model="registration.email" 
                                            id="email" 
                                            name="email" 
                                            placeholder="Seu email"
                                            required
                                            >
                                        </b-form-input>
                                </b-col>
                                <b-col md="5">    
                                        <p class="label-input-due mt-3">Seu nome</p>
                                        <b-form-input 
                                            class="form-due" 
                                            v-model="registration.phone" 
                                            id="phone" 
                                            name="phone" 
                                            placeholder="Celular"
                                            required
                                            >
                                        </b-form-input>
                                </b-col>
                                <b-col md="7">    
                                        <p class="label-input-due mt-3">Seu nome</p>
                                        <b-form-input 
                                            class="form-due" 
                                            v-model="registration.company" 
                                            id="company" 
                                            name="company" 
                                            placeholder="Nome da Empresa"
                                            required
                                            >
                                        </b-form-input>
                                </b-col >
                                <b-col md="5">    
                                        <p class="label-input-due mt-3">Seu nome</p>
                                        <b-form-select 
                                            class="form-due" 
                                            v-model="registration.employees" 
                                            :options="options" 
                                            id="employees" 
                                            name="employees" 
                                            placeholder="Qtd. de Funcionários"
                                            required
                                            >
                                        </b-form-select>
                                </b-col>
                                <b-col md="7">    
                                        <p class="label-input-due mt-3">Seu nome</p>
                                        <b-form-input 
                                            class="form-due" 
                                            v-model="registration.site" 
                                            id="site" 
                                            name="site" 
                                            placeholder="http://"
                                            required
                                            >
                                        </b-form-input>
                                </b-col>
                                <b-col data-netlify-recaptcha="true">
                                </b-col>
                            </b-row> 
                            <b-row>
                                <b-col align="right" class="mt-3"><p>{{registration}}</p>
                                    <b-button class="pri-btn pri-btn-prev ml-md-3" @click.prevent="prev()" >Texto Botão</b-button>
                                    <b-button class="sec-btn ml-md-3  ml-sm-3" type="submit">Texto Botão</b-button>
                                </b-col>
                            </b-row>
                        </b-col>
                    </b-col>
                </b-form>
            </b-row>
        </b-modal>
    
</template>