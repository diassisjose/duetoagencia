<template>
    <b-container>
        <no-ssr>
            <b-row>
                <b-col cols="3">
                    <h3>Chamada de Título</h3>
                    <p>Descrição</p>
                    <div class="mt-3">
                        <strong>{{ selected1 }}</strong><br>   
                        <strong>{{ selected2 }}</strong><br>  
                        <strong>{{ selected3 }}</strong><br>
                        <strong>{{ selected4 }}</strong><br>
                        <strong>{{ selected5 }}</strong><br>
                        <strong>{{ selected6 }}</strong><br> 
                    </div>
                    <h3>R$</h3>
                </b-col>
                <b-col cols="9">
                    <b-card no-body>
                        <b-tabs pills card vertical>
                            <b-tab title="Tab 1" active>
                                <b-card-text>
                                    <h3>Chamada de Título</h3>
                                    <p>Descrição</p>
                                    <b-form-group label="Individual radios">
                                      <b-form-radio v-model="selected1" name="some-radios" value="50">Option A</b-form-radio>
                                      <b-form-radio v-model="selected1" name="some-radios" value="64">Option B</b-form-radio>
                                      <b-form-radio v-model="selected1" name="some-radios" value="1245">Option C</b-form-radio>
                                    </b-form-group>
                                </b-card-text>
                            </b-tab>
                            <b-tab title="Tab 2">
                                <b-card-text>
                                    <h3>Chamada de Título</h3>
                                    <p>Descrição</p>
                                    <b-form-group label="Individual radios">
                                      <b-form-radio v-model="selected2" name="some-radios" value="A1">Option A1</b-form-radio>
                                      <b-form-radio v-model="selected2" name="some-radios" value="B1">Option B1</b-form-radio>
                                      <b-form-radio v-model="selected2" name="some-radios" value="C1">Option C1</b-form-radio>
                                    </b-form-group>
                                </b-card-text>
                            </b-tab>
                            <b-tab title="Tab 3">
                                <b-card-text>
                                    <h3>Chamada de Título</h3>
                                    <p>Descrição</p>
                                    <b-form-group label="Individual radios">
                                      <b-form-radio v-model="selected3" name="some-radios" value="A2">Option A2</b-form-radio>
                                      <b-form-radio v-model="selected3" name="some-radios" value="B2">Option B2</b-form-radio>
                                      <b-form-radio v-model="selected3" name="some-radios" value="C2">Option C2</b-form-radio>
                                    </b-form-group>
                                </b-card-text>
                            </b-tab>
                            <b-tab title="Tab 4">
                                <b-card-text>
                                    <h3>Chamada de Título</h3>
                                    <p>Descrição</p>
                                    <b-form-group label="Individual radios">
                                      <b-form-radio v-model="selected4" name="some-radios" value="A3">Option A2</b-form-radio>
                                      <b-form-radio v-model="selected4" name="some-radios" value="B3">Option B2</b-form-radio>
                                      <b-form-radio v-model="selected4" name="some-radios" value="C3">Option C2</b-form-radio>
                                    </b-form-group>
                                </b-card-text>
                            </b-tab>
                            <b-tab title="Tab 5">
                                <b-card-text>
                                    <h3>Chamada de Título</h3>
                                    <p>Descrição</p>
                                    <b-form-group label="Individual radios">
                                      <b-form-radio v-model="selected5" name="some-radios" value="A4">Option A2</b-form-radio>
                                      <b-form-radio v-model="selected5" name="some-radios" value="B4">Option B2</b-form-radio>
                                      <b-form-radio v-model="selected5" name="some-radios" value="C4">Option C2</b-form-radio>
                                    </b-form-group>
                                </b-card-text>
                            </b-tab>
                            <b-tab title="Tab 6">
                                <b-card-text>
                                    <h3>Chamada de Título</h3>
                                    <p>Descrição</p>
                                    <b-form-group label="Individual radios">
                                      <b-form-radio v-model="selected6" name="some-radios" value="A5">Option A2</b-form-radio>
                                      <b-form-radio v-model="selected6" name="some-radios" value="B5">Option B2</b-form-radio>
                                      <b-form-radio v-model="selected6" name="some-radios" value="C5">Option C2</b-form-radio>
                                    </b-form-group>
                                </b-card-text>
                            </b-tab>
                        </b-tabs>
                        
                    </b-card>
                </b-col>
            </b-row>
        </no-ssr>
    </b-container>
</template>
<script>
  export default {
    data() {
        
        return {
          selected1: '',
          selected2: '',
          selected3: '',
          selected4: '',
          selected5: '',
          selected6: '',
        }
    }
  }
</script>