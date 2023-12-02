<template>
  <button @click="logout" class="btn btn-secondary">Sair</button>
</template>

<script>
export default {
  methods: {
    logout() {
      // Limpa o token do localStorage
      localStorage.removeItem('token');
      
      this.$router.push('/');
    }
  }
};
</script>