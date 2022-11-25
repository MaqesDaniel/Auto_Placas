<template>
    <div class="Container">
      <div class="Content">
        <div class="mainContent">
        
          <div class="card-header">
            <h1 class="header-title">Estoque de Acessórios</h1>
          </div>
          
          <div class="card-body">
          <select class="select-form-control" v-model="selected">
            <option value="undefined" disabled>Selecione a Loja</option>
            <option>São Luís</option>
            <option>Bacabal</option>
            <option>Balsas</option>
            <option>Imperatriz</option>
            <option>Açailândia</option>
            <option>Santa Inês</option>
          </select>
          <input class="btn-primary" type="submit" value="Filtrar"/>
        </div>
        
        <div class="col-6-body">
          <div class="col-6">
          <table class="value-card">
            <tbody class="value-card-body">
              <tr class="col-6-container">
                <th class="col-6-text">Total de Suporte para Moto:</th>
                <td class="col-6-value">200</td>
              </tr>
              
              <tr class="col-6-content">
                <th class="col-6-text">Total de Travas de Suporte para Moto:</th>
                <td class="col-6-value">500</td>
              </tr>

              <tr class="col-6-content">
                <th class="col-6-text">Valor dos Produtos em Estoque (preço de custo):</th>
                <td class="col-6-value" 
                style="
                    width: 100px;
                    height: 32px;
                    padding: 6px;
                    border-radius: 4px;
                    margin-right: 8px;
                    border-width: 0;
                    background-color: #00D27A;
                    color: white;
                    font-size: 16px;
                    font-weight: 700;
                "
                >R$ 7.200,00</td>
              </tr>
            </tbody>
          </table>
        </div>
  
        <div class="col-6">
          <table class="value-card">
            <tbody class="value-card-body">
              <tr class="col-6-container">
                <th class="col-6-text">Total de Suporte para Carro:</th>
                <td class="col-6-value">350</td>
              </tr>
              
              <tr class="col-6-content">
                <th class="col-6-text">Total de Travas de Suporte para Carro:</th>
                <td class="col-6-value">1.000</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
        
      <div class="col-12-body">
          <div class="col-12">
            <table class="col-12-card">
              <thead>
                <tr>
                  <th class="equipment-title">Acessório:</th>
                  <th class="equipment-title">Quantidade:</th>
                </tr>
              </thead>
  
              <tbody>
                <tr>
                  <td class="equipment-name">SUPORTE PARA CARRO</td>
                  <td class="equipment-quantity">200</td>
                </tr>
  
                <tr>
                  <td class="equipment-name">SUPORTE PARA MOTO</td>
                  <td class="equipment-quantity">380</td>
                </tr>
  
                <tr>
                  <td class="equipment-name">LACRE CARRO - LISO</td>
                  <td class="equipment-quantity">150</td>
                </tr>
  
                <tr>
                  <td class="equipment-name">LACRE PERSONALIZADO (MOTO) - FLAMENGO</td>
                  <td class="equipment-quantity">200</td>
                </tr>
  
                <tr>
                  <td class="equipment-name">LACRE PERSONALIZADO (CARRO) - GUARDA-ME Ó DEUS POIS EM TI EU CONFIO</td>
                  <td class="equipment-quantity">45</td>
                </tr>
  
                <tr>
                  <td class="equipment-name">LACRE PERSONALIZADO (MOTO) - UMA VEZ FLAMENGO, SEMPRE FLAMENGO</td>
                  <td class="equipment-quantity">18</td>
                </tr>
  
                <tr>
                  <td class="equipment-name">LACRE PERSONALIZADO (CARRO) - RAPOSA</td>
                  <td class="equipment-quantity">8</td>
                </tr>
  
                <tr>
                  <td class="equipment-name">LACRE PERSONALIZADO (CARRO) - IMPERATRIZ</td>
                  <td class="equipment-quantity">96</td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
  </div>
  </template>
  
  <script>
  export default {
    name: 'RelatorioAcessorios',
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  
  .Container{
    background-color: #D8E2EF;
    padding: 8px 6px;
  }
  .Content{
    background-color: white;
  }
  
  .card-header{
    width: max-content;
    padding: 8px 20px;
  }
  .header-title {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-weight: 500;
    font-size: 20px;
    color: #344050;
  }
  .card-body{
    height: 40px;
    padding: 8px 20px;
    margin-bottom: 12px;
  }
  .select-form-control{
    width: 25%;
    height: 40px;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 20px;
    font-weight: 400;
    padding: 0px 4px;
    border-radius: 4px;
    border-color: #D8E2EF;
    border-width: 2px;
    margin-right: 8px;
    color: gray;
    background-color: white;
  }
  .date-form-control {
    width: 20%;
    height: 36px;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 20px;
    font-weight: 400;
    padding: 0px 4px;
    border-radius: 4px;
    border-color: #D8E2EF;
    border-style: solid;
    border-width: 2px;
    margin-right: 8px;
    color: gray;
  }
  .btn-primary{
    width: 84px;
    height: 36px;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 20px;
    font-weight: 400;
    padding: 2px 4px;
    border-radius: 4px;
    margin-right: 8px;
    border-width: 0;
    background-color: #2C7BE5;
    color: white;
  }
  .btn-primary:hover{
    width: 84px;
    height: 36px;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 20px;
    font-weight: 400;
    padding: 2px 4px;
    border-radius: 4px;
    margin-right: 8px;
    border-width: 0;
    background-color: #2063ba;
    color: white;
  }
  .col-6-body{
    display: flex;
    flex-direction: row;
    margin-left: 30px;
  }
  .col-6{
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-weight: 400;
    font-size: 16px;
  }
  .value-card{
    width: 50%;
    margin-bottom: 8px; 
  }
  .col-6-container{
    display: flex;
    flex-direction: row;
    border-bottom: 2px solid #D8E2EF;
  }
  .col-6-content{
    display: flex;
    flex-direction: row;
  }
  .col-6-text{
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 16px;
    font-weight: bold;
    color: #4D5969;
    margin: 8px 0px;
    width: 380px;
    text-align: left;
  }
  .col-6-value{
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 16px;
    color: #4D5969;  
    margin: 10px 5px 0px 200px;
    width: 200px;
  }
  .col-12-body{
    display: flex;
    flex-direction: row;
    margin-left: 30px;
  }
  .col-12-card{
    width: 1400px;
    margin-bottom: 12px;
  }
  .equipment-title{
    width: 85%;
    height: 32px;
    margin-bottom: 8px;
    padding-left: 8px;
    background-color: #EDF2F9;
    text-align: left;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 14px;
    color: #4D5969; 
  }
  .equipment-name{
    width: 85%;
    height: 32px;
    margin-bottom: 8px;
    text-align: left;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 16px;
    color: #6d757d;
    border-bottom: 2px solid #EDF2F9; 
  }
  .equipment-quantity{
    width: 30%;
    height: 32px;
    margin-bottom: 8px;
    text-align: left;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 16px;
    color: #6d757d; 
    border-bottom: 2px solid #EDF2F9; 
  
  }
  </style>
  