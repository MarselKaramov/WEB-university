<script></script>

<template>
	<form @submit.prevent>
		<h1>Создание заявки</h1>
		
		<label for="title">Тема, 5–80 символов</label>
		<input id="title" name="title" autofocus>

		<label for="number">Номер заявки</label>
		<input id="number" name="number" type="number">

		<label for="description">Описание, 10–500 символов</label>
		<textarea id="description" name="description"></textarea>

		<button type="submit">Создать</button>
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
  input,
  textarea {
    padding: 6px 10px;
    border: 1px solid #93c5fd;
    border-radius: 4px;
    outline: none;
    font-family: inherit;
  }
  textarea {
    min-height: 80px;
    resize: vertical;
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