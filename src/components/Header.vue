<template>
  <div class="header">
    <h1>{{ title }}</h1>
    <div class="message">
      <p>{{ message }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    title: {
      type: String,
      default: 'Vai Corinthians!'
    },
    message: {
      type: String,
      default: 'VAI CORINTHIANS!'
    },
    imageUrl: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.header {
  text-align: center; /* Centraliza o texto */
  padding: 20px;
  background-image: url(''); /* Imagem será definida via props */
  background-size: 10; /* Diminui o tamanho da imagem */
  background-repeat: no-repeat; /* Evita que a imagem se repita */
  background-position: center;
  color: white; /* Cor do texto */
  height: 200px; /* Altura definida para o cabeçalho */
}

h1 {
  font-size: 3rem; /* Aumenta o tamanho do texto */
  margin: 0; /* Remove margens padrão */
}

.message {
  background-color: rgba(0, 0, 0, 0.5); /* Fundo semi-transparente para a mensagem */
  padding: 10px; /* Espaçamento interno */
}

.message p {
  font-size: 1.5rem; /* Tamanho da mensagem */
  margin: 0; /* Remove margens padrão */
}
</style>