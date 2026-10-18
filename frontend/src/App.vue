<script setup>
import { ref } from 'vue'
import CreateFormScreen from './screens/CreateFormScreen.vue'
import ItemsScreen from './screens/ItemsScreen.vue'
import LoginScreen from './screens/LoginScreen.vue'

const screen = ref('login')

</script>

<template>
  <header>
    <button @click="screen = 'login'">Авторизация</button>
    <button @click="screen = 'create'">Создание заявки</button>
    <button @click="screen = 'list'">Список</button>
  </header>

  <main>
    <LoginScreen v-if="screen === 'login'"/>
    <CreateFormScreen v-else-if="screen === 'create'"/>
    <ItemsScreen v-else-if="screen === 'list'"/>
  </main>
</template>

<style scoped>
header {
  margin-bottom: 10px;
}
</style>