<template>
    <VendasAcessorios/>
    <RelatorioAcessorios/>
</template>

<script>
import VendasAcessorios from './components/rel_vendas/vendasAcessorios.vue'
import RelatorioAcessorios from './components/rel_estoque/relatorioAcessorios.vue'

export default {
  name: 'App',
  components: {
    VendasAcessorios,
    RelatorioAcessorios
  }
}
</script>

<style>
* {
  padding: 0px; 
  margin:0px; 
  box-sizing: border-box}
</style>
