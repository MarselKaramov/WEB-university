<script setup>
	const items = [
    { id: 1, number: 'A-101', title: 'Насос не запускается', siteId: 2, status: 'New' },
    { id: 2, number: 'A-102', title: 'Проверить вентиль', siteId: 1, status: 'InProgress' }
  ]
</script>

<template>
	<table>
    <thead>
      <tr>
        <th>ID</th>
        <th>Номер заявка</th>
        <th>Заголовок</th>
        <th>Site ID</th>
        <th>Статус</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="item in items" :key="item.id">
        <td>{{ item.id }}</td>
        <td>{{ item.number }}</td>
        <td>{{ item.title }}</td>
        <td>{{ item.siteId }}</td>
        <td>{{ item.status }}</td>
      </tr>
    </tbody>
  </table>
</template>

<style scoped>
table {
    border-collapse: collapse;
    width: 100%;
  }
  th,
  td {
    padding: 8px 12px;
    border: 1px solid #93c5fd;
    text-align: left;
  }
  th {
    color: #fff;
    background: #4970dd;
  }

</style>