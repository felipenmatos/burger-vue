<template>
  <p>Banner Form component</p>
  <div>
    <form id="burger-form">
      <div class="input-container">
        <label for="nome">Nome do cliente:</label>
        <input
          type="text"
          id="nome"
          name="nome"
          v-model="nome"
          placeholder="Digite o seu nome"
        />
      </div>
      <div class="input-container">
        <label for="pao">Escolha o pão:</label>
        <select name="pao" id="pao" v-model="pao">
          <option value="">Selecione o seu pão</option>
          <option value="integral">Integral</option>
        </select>
      </div>
      <div class="input-container">
        <label for="carne">Escolha a carne do seu Burger:</label>
        <select name="carne" id="carne" v-model="carne">
          <option value="">Selecione a carne</option>
          <option value="maminha">Maminha</option>
        </select>
      </div>
      <div class="input-container">
        <label for="opcionais">Selecione os opcionais:</label>
        <div class="checkbox-container">
          <input
            type="checkbox"
            name="opcionais"
            v-model="opcionais"
            value="salame"
          />
          <span>Salame</span>
        </div>
        <div class="input-container">
          <input type="submit" class="submit-btn" value="Criar meu Burger" />
        </div>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "BurgerForm",
};
</script>

<style scoped></style>
