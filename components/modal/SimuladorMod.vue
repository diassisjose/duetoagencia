<template>
  <b-modal class="modaldue" hide-footer id="modal-1" size="xl">
    <b-col class="modal-title">
      <h3 class="h-modal">Seu Plano Digital sob demanda:</h3>
      <h5 class="h5-modal">
        Selecione os planos que quer receber em seu orçamento!
      </h5>
    </b-col>
    <b-form
      name="form-leads"
      action="POST"
      method="post"
      data-netlify="true"
      data-netlify-recaptcha="true"
      data-netlify-honeypot="bot-field"
      class="mx-4"
    >
      <input type="hidden" name="form-name" value="form-leads" />
      <b-row>
        <b-col md="7" class="mx-4">
          <b-row>
            <b-col
              class="switchdeact mx-1 my-1"
              v-on:click="
                registration.checkedPlan1 = !registration.checkedPlan1
              "
              :class="{ checked: registration.checkedPlan1 }"
            >
              <input
                class="footer-switch"
                type="checkbox"
                value="socialMedia"
                name="socialMedia"
                id="socialMedia"
                v-model="registration.checkedPlan1"
                align="left"
              />

              <h4 class="h-switch">Imagens e Vídeos para Redes Sociais</h4>
              <p class="p-switch">
                Conteúdo criativo para encantar seu público
              </p>
            </b-col>
            <b-col
              class="switchdeact mx-1 my-1"
              v-on:click="
                registration.checkedPlan2 = !registration.checkedPlan2
              "
              :class="{ checked: registration.checkedPlan2 }"
            >
              <input
                class="footer-switch"
                type="checkbox"
                value="managerSocial"
                name="managerSocial"
                id="managerSocial"
                v-model="registration.checkedPlan2"
              />
              <h4 class="h-switch">Plano de Gestão nas Redes Sociais</h4>
              <p class="p-switch">Gestão e Planejamento da imagem digital</p>
            </b-col>
            <b-col
              class="switchdeact mx-1 my-1"
              v-on:click="
                registration.checkedPlan3 = !registration.checkedPlan3
              "
              :class="{ checked: registration.checkedPlan3 }"
            >
              <input
                class="footer-switch"
                type="checkbox"
                value="socialAds"
                name="socialAds"
                id="socialAds"
                v-model="registration.checkedPlan3"
              />
              <h4 class="h-switch">Anúncios em Canais Digitais</h4>
              <p class="p-switch">Anúncios para captar e converter</p>
            </b-col>
            <b-col
              class="switchdeact mx-1 my-1"
              v-on:click="
                registration.checkedPlan4 = !registration.checkedPlan4
              "
              :class="{ checked: registration.checkedPlan4 }"
            >
              <input
                class="footer-switch"
                type="checkbox"
                value="inboundMkt"
                name="inboundMkt"
                id="inboundMkt"
                v-model="registration.checkedPlan4"
              />
              <h4 class="h-switch">Planejamento Inbound Marketing</h4>
              <p class="p-switch">Estratégia para fidelizar clientes</p>
            </b-col>
            <b-col
              class="switchdeact mx-1 my-1"
              v-on:click="
                registration.checkedPlan5 = !registration.checkedPlan5
              "
              :class="{ checked: registration.checkedPlan5 }"
            >
              <input
                class="footer-switch"
                type="checkbox"
                value="emailMkt"
                name="emailMkt"
                id="emailMkt"
                v-model="registration.checkedPlan5"
              />
              <h4 class="h-switch">Relacionamento com Email Mkt</h4>
              <p class="p-switch">Conquiste e informe de forma cíclica.</p>
            </b-col>
            <b-col
              class="switchdeact mx-1 my-1"
              v-on:click="
                registration.checkedPlan6 = !registration.checkedPlan6
              "
              :class="{ checked: registration.checkedPlan6 }"
            >
              <input
                class="footer-switch"
                type="checkbox"
                value="webDev"
                name="webDev"
                id="webDev"
                v-model="registration.checkedPlan6"
              />
              <h4 class="h-switch">Criação de Site e Aplicativo</h4>
              <p class="p-switch">Sua empresa aberta 24h</p>
            </b-col>
          </b-row>
        </b-col>
        <b-col>
          <b-row>
            <b-col class="pt-sm-5 pt-md-0 mx-md-3 px-sm-2">
              <p class="label-input-due mt-2">Seu nome</p>
              <b-form-input
                class="form-due"
                v-model="registration.name"
                id="name"
                name="name"
                placeholder="Seu nome"
                required
              >
              </b-form-input>
              <p class="label-input-due mt-2">Seu email</p>
              <b-form-input
                class="form-due"
                v-model="registration.email"
                id="email"
                name="email"
                placeholder="Seu email"
                required
              >
              </b-form-input>
              <p class="label-input-due mt-2">Nome da Empresa</p>
              <b-form-input
                class="form-due"
                v-model="registration.company"
                id="company"
                name="company"
                placeholder="Nome da Empresa"
                required
              >
              </b-form-input>
              <p class="label-input-due mt-2">Funcionários</p>
              <b-form-select
                class="form-due"
                v-model="registration.employees"
                :options="options"
                id="employees"
                name="employees"
                placeholder="Quantos?"
                required
              >
              </b-form-select>
              <p class="label-input-due mt-2">Seu site</p>
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

            <!-- <b-row align="right" class="mt-3">
                             <p>{{registration}}</p>
                        </b-row> -->
          </b-row>
          <b-row align="center">
            <b-col class="mt-2" data-netlify-recaptcha="true"></b-col>
            <b-col>
              <b-button class="sec-btn mt-3" type="submit">Finalizar</b-button>
            </b-col>
          </b-row>
        </b-col>
      </b-row>
    </b-form>
  </b-modal>
</template>

<script>
import SwitchChk from "~/components/switch/SwChecked";
import InputModal from "~/components/modal/InputModal";
export default {
  components: {
    SwitchChk,
    InputModal,
  },
  data() {
    return {
      step: 1,
      registration: {
        checkedPlan1: false,
        checkedPlan2: false,
        checkedPlan3: false,
        checkedPlan4: false,
        checkedPlan5: false,
        checkedPlan6: false,

        name: null,
        email: null,
        phone: null,
        company: null,
        employees: null,
        site: "https://",
      },
      employees: null,
      options: [
        { value: null, text: "Quantos funcionários" },
        { value: "a", text: "1" },
        { value: "b", text: "2 a 5" },
        { value: "c", text: "6 a 10" },
        { value: "d", text: "11 a 50" },
        { value: "e", text: "Acima de 50" },
      ],
    };
  },
  methods: {
    submit(evt) {
      evt.preventDefault();
      alert(JSON.stringify(this.registration));
    },
    // onReset(evt) {
    //   evt.preventDefault()
    //   // Reset our form values
    //   this.form.email = ''
    //   this.form.name = ''
    //   this.form.food = null
    //   this.form.checked = []
    //   // Trick to reset/clear native browser form validation state
    //   this.show = false
    //   this.$nextTick(() => {
    //     this.show = true
    //   })
    // }
  },
};
</script>
