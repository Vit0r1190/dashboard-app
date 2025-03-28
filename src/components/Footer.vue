<template>
  <div class="footer">
    <p>{{ footerText }}</p>
    <img :src="imageUrl" alt="Imagem do Rodapé" class="footer-image" />
  </div>
</template>

<script>
export default {
  name: 'Footer',
  props: {
    footerText: {
      type: String,
      default: '© 2023 Todos os direitos reservados.'
    },
    imageUrl: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.footer {
  text-align: center; /* Centraliza o texto */
  padding: 20px;
  color: white; /* Cor do texto */
}

.footer-image {
  max-width: 280x; /* Aumenta a largura máxima da imagem */
  height: auto; /* Mantém a proporção da imagem */
  margin-top: 10px; /* Espaço acima da imagem */
}
</style>