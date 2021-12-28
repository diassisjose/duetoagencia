<template>
  <b-row class="mb-5"  >
    <b-col cols="12">
      <h2 class="h-header mx-md-5 mb-3 px-md-5" align="center">Principais benefícios <br>em ser nosso cliente:</h2>
      <hr class="hr-due mb-5" align="center">
    </b-col>
    
    <b-col role="tablist" sm md lg>
      <b-col no-body>
        <b-col header-tag="header" class="p-1" role="tab">
          <b-button block href="#" v-b-toggle.accordion-1 class="tablist-due">{{ question1 }} 
            <i class="icon ion-md-arrow-dropdown rotate icon-top"></i>
          </b-button>
        </b-col>
        <b-collapse id="accordion-1" accordion="my-accordion" role="tabpanel">
          <b-col>
            <p class="ml-2 pb-3 pt-3 p-card px-md-4"><i class="icon ion-md-tablet-portrait rotate"></i><br>{{ text1 }}</p>
          </b-col>
        </b-collapse>
      </b-col>
      <b-col no-body>
        <b-col header-tag="header" class="p-1" role="tab">
          <b-button block href="#" v-b-toggle.accordion-2 class="tablist-due">{{ question2 }} <i class="icon ion-md-arrow-dropdown rotate icon-top"></i></b-button>
        </b-col>
        <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
          <b-col>
            <p class="ml-2 pb-3 pt-3 p-card px-md-4"><i class="icon ion-md-contacts rotate"></i><br>{{ text2 }}</p>
          </b-col>
        </b-collapse>
      </b-col>
      <b-col no-body>
        <b-col header-tag="header" class="p-1" role="tab">
          <b-button block href="#" v-b-toggle.accordion-3 class="tablist-due">{{ question3 }} <i class="icon ion-md-arrow-dropdown rotate icon-top"></i></b-button>
        </b-col>
        <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
          <b-col>
            <p class="ml-2 pb-3 pt-3 p-card px-md-4"><i class="icon ion-md-finger-print rotate"></i><br>{{ text3 }}</p>
          </b-col>
        </b-collapse>
      </b-col>
    </b-col>
    <b-col role="tablist" sm md lg>
      <b-col no-body>
        <b-col header-tag="header" class="p-1" role="tab">
          <b-button block href="#" v-b-toggle.accordion-4 class="tablist-due">{{ question4 }} <i class="icon ion-md-arrow-dropdown rotate icon-top"></i></b-button>
        </b-col>
        <b-collapse id="accordion-4" accordion="my-accordion" role="tabpanel">
          <b-col>
            <p class="ml-2 pb-3 pt-3 p-card px-md-4"><i class="icon ion-md-cash rotate"></i><br>{{ text4 }}</p>
          </b-col>
        </b-collapse>
      </b-col>
      <b-col no-body>
        <b-col header-tag="header" class="p-1" role="tab">
          <b-button block href="#" v-b-toggle.accordion-5 class="tablist-due">{{ question5 }} <i class="icon ion-md-arrow-dropdown rotate icon-top"></i></b-button>
        </b-col>
        <b-collapse id="accordion-5" accordion="my-accordion" role="tabpanel">
          <b-col>
            <p class="ml-2 pb-3 pt-3 p-card px-md-4"><i class="icon ion-md-trending-up rotate"></i><br>{{ text5 }}</p>
          </b-col>
        </b-collapse>
      </b-col>
      <b-col no-body>
        <b-col header-tag="header" class="p-1" role="tab">
          <b-button block href="#" v-b-toggle.accordion-6 class="tablist-due">{{ question6 }} <i class="icon ion-md-arrow-dropdown rotate icon-top"></i></b-button>
        </b-col>
        <b-collapse id="accordion-6" accordion="my-accordion" role="tabpanel">
          <b-col>
            <p class="ml-2 pb-3 pt-3 p-card px-md-4"><i class="icon ion-md-git-network rotate"></i><br>{{ text6 }}</p>
          </b-col>
        </b-collapse>
      </b-col>
    </b-col>
  </b-row>
</template>

<script>
  export default {
    data() {
      return {
        question1: `1. Ter uma presença online para ser encontrado`,
        text1: `
          A cada novo conteúdo que você publica, independente do seu formato escolhido, 
          mais oportunidades você tem de ser encontrado pelos internautas e futuros clientes.
          É uma questão um pouco lógica falar disso, mas pense como se você fosse um time 
          de futebol: quanto mais você treina e joga, mais preparado você fica.
          E, na mesma proporção, maiores suas chances de obter vitórias e ganhos.
        `,
        question2: `2. Gerar relacionamento com o cliente`,
        text2: `
          Por que fazer marketing de conteúdo no Brasil? Simplesmente para se relacionar melhor 
          com o seu cliente – essa resposta já bastaria para todo esse conteúdo.
          Quando você cria bons conteúdos, em diversos canais de comunicação, você dá 
          às pessoas motivos para confiarem e interagirem com você.
          O resultado e um relacionamento mais próximo, mais saudável e mais confiável.
        `,
        question3: `3. Aumentar o engajamento com a sua marca`,
        text3: `
          Esse tópico é apenas para complementar o anterior e também explica 
          para que serve o marketing de conteúdo. O engajamento com a marca, 
          que tanto se fala em marketing digital, é sobre os seus clientes e 
          possíveis clientes estarem ligados ao seu produto. Resumindo: o marketing 
          de conteúdo, quando feito com qualidade e valor, aumenta o engajamento 
          com a marca, fidelizando os clientes.
        `,
        question4: `4. Facilitar as oportunidades de vendas`,
        text4: `
          Então, o fato mais importante disso é que você, com o marketing de conteúdo, 
          pode “ensinar” seus clientes sobre os benefícios de se comprar alguns produtos. 
          Isso tem a ver com a geração de leads também. Se você consegue atrair pessoas 
          ao falar sobre a nova propriedade de um tênis que vai ajudar os atletas e 
          manterem seus pés mais confortáveis em corridas de longo percurso...
          Eles vão ficar interessados nisso e vão querer saber mais.
        `,
        question5: `5. Baixo investimento, mas grandes resultados.`,
        text5: `
          Faça os cálculos, se você comparar o valor usado em mídias tradicionais com o 
          valor investido no Marketing Digital, vai concluir que é mais econômico investir 
          no meio digital.  Pois se utilizado em um outdoor, por exemplo, vai  atingir um 
          grande número de pessoas, mas não vai conseguir segmentar o público.
          Em uma ação digital, você consegue atingir a quantidade de pessoas que você 
          quiser e ainda segmentar seu público-alvo, definindo a idade ideal, profissão,
           entre outros aspectos.
        `,
        question6: `6. Entender o comportamento do consumidor`,
        text6: `
          O consumidor mudou muito nos últimos anos, ele não se interessa apenas pelo produto, 
          mas ‘por toda a experiência’ que vai ter ao realizar determinada  compra. No 
          Marketing Digital, você pode proporcionar experiências para o seu público alvo, 
          como oferecer comunicação online entre o consumidor e a empresa, e também permitir 
          uma boa usabilidade com um site intuitivo. #ficaAdica
          As tendências para 2019 envolvem a utilização correta de estratégias de SEO, com o 
          objetivo de atrair cada vez mais atenção e proporcionar experiências inovadoras 
          para os usuários. A produção de conteúdos relevantes continuará sendo a chave 
          para Rankear as melhores posições no Google. Se você quer colher bons frutos com o 
          Marketing Digital, aposte em pensar na experiência do consumidor, não basta apenas 
          desenvolver estratégias, é necessário se colocar no lugar do seu público alvo 
          para atraí-lo da forma certa.
        `
      }
    }
  }
</script>