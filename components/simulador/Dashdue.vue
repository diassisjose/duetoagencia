<template>
    <no-ssr>
        <b-col>
           
        </b-col>
    
    </no-ssr>
</template>

<script>
  export default {
      data: function() {
          return {
          title: 'Relatório de Vendas',
          sales: null,
          }
      },
      methods: {
          getSales() {
              fetch('/application/sales.json')
                .then(resp => resp.json())
                .then(data => console.log(data))
          }
      },
      mounted() {
          this.getSales()
      },
  }
</script>
