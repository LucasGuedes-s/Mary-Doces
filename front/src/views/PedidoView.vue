<template>
  <div class="about">
    <NavBar />
  </div>
  <div class="conteiner">
    <form action="">
      <div class="text">
        <label>Nome do solicitante: </label>
        <input type="text" placeholder="ex: José Dantas" required>
      </div>
      <div>
        <label>Pedido: </label>
        <input type="text" name="pedido" placeholder="ex: Bolo para festa" id="pedido" required>
      </div>
      <div>
        <label>Cidade de entrega: </label>
        <select>
          <option>Cidade de entrega</option>
          <option>Acari</option>
          <option>Currais Novos</option>
          <option>Cruzeta</option>
          <option>Jardim do Seridó</option>
        </select>
      </div>
      <div>
        <label>Endereço de entrega: </label>
        <input type="text" name="endereco" placeholder="ex: Rua Horácio Pires, Nº52" id="endereco" required>
      </div>
      
      <div>
        <label>Data de entrega: </label>
        <input type="datetime-local" required>
      </div>
      <div class="text">
        <label>Observações: </label>
        <input type="text">
      </div>
      <div>
        <button type="submit">Finalizar pedido</button>
      </div>
    </form>
  </div>
  <div class="img-pedidos">
    <img  src="@/assets/imagem.png"> 
  </div>
</template>
<script>
import NavBar from '@/components/NavBar.vue';
  export default {
    name: 'PedidosView',
    data(){
    },
    components: {
      NavBar,
    }
  }
</script>
<style>
  .img-pedidos img {
    max-width: 40%;
    height: auto;
    margin-left: 20px;
    margin-top: 50px;

  }
  .conteiner {
    margin: 70px;
    margin-top: 150px;
    float: left;
    width: 40%;
    background-color: #f8f8f8;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    text-align: left;
    overflow: hidden; /* Adicionando overflow para conter o float */
  }

  form {
    margin-bottom: 20px;
  }

  .text,
  div {
    margin-bottom: 10px;
  }

  label {
    display: inline-block;
    width: 150px;
    font-weight: bold;
  }
  select{
    width: 370px;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 3px;
    font-size: 14px;
  }

  input[type="text"],
  input[type="datetime-local"] {
    width: 350px;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 3px;
    font-size: 14px;
  }
  button {
    display: block;
    width: 97%;
    margin-top: 10px;
    padding: 10px;
    background-color: #9666ca;
    color: #ffffff;
    font-weight: bold;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }

</style>