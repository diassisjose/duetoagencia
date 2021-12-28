<template>
  <b-navbar class="py-3 px-md-5 nav-border-due" sticky toggleable="lg" type="dark">
    <b-navbar-brand href="/"><img src="~/assets/img/logo-w-dueto.png" width="181" alt=""></b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav class="ml-5 ml-auto">
        <b-nav-item class="nav-link-due navdue-dec" href="/#howdoes">Como funciona</b-nav-item>
        <b-nav-item class="nav-link-due navdue-dec" href="/#solutions">Soluções</b-nav-item>
        <b-nav-item class="nav-link-due navdue-dec" href="/#benefits">Benefícios</b-nav-item>
      </b-navbar-nav>
      <b-navbar-nav>
        <b-button class="btn-purple effect-button ml-md-3" v-b-modal.modal-1 >Quero orçamento!</b-button>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>