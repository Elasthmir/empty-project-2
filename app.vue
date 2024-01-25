<script setup>
const openChat = ref(false)
const toggle = () => {
  openChat.value = !openChat.value
}
</script>
<template>
  <div>
    <NuxtLayout>
      <div class="body-content">
        <NuxtPage />
      </div>
    </NuxtLayout>
    <div class="chatOpen" @click="toggle" v-if="openChat"></div>
    <div class="chatClose" @click="toggle" v-else></div>

  </div>
</template>
<style scoped>
.chatClose {
  z-index: 999999999;
  width: 50px;
  height: 50px;
  background-color: #3498db;
  /* Kolor tła */
  border-radius: 50%;
  /* Ustala kształt koła */
  position: fixed;
  /* Pozycja absolutna */
  bottom: 0;
  /* Odległość od dołu */
  right: 0;
  /* Odległość od prawej */
}

.chatOpen {
  z-index: 999999999;
  width: 50px;
  height: 150px;
  background-color: #3498db;
  /* Kolor tła */
  position: fixed;
  /* Pozycja absolutna */
  bottom: 0;
  /* Odległość od dołu */
  right: 0;
  /* Odległość od prawej */
}
</style>