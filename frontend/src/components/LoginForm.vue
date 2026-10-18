<script></script>

<template >
	<form @submit.prevent>
		<h1>Вход</h1>
		
		<label for="login">Логин</label>
		<input id="login" name="login" autofocus>

		<label for="pass">Пароль</label>
		<input id="pass" name="pass" autofocus>

		<button>Войти</button>
	</form>
</template>

<style scoped>
	 h1 {
    margin: 0;
    color: #4970dd;
  }
  form {
    width: 50%;
    display: flex;
    flex-direction: column;
    gap: 5px;
  }
  input {
    padding: 6px 10px;
    border: 1px solid #93c5fd;
    border-radius: 4px;
    outline: none;
  }
  button {
    margin-top: 5px;
    padding: 6px 10px;
    color: #fff;
    background: #4970dd;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
</style>