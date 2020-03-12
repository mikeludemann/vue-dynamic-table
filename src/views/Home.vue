<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <DynamicTable :datas="[{ id: 1, name: 'John Doe', age: 21, email: 'john.doe@email.com' }, { id: 2, name: 'Mary Doe', age: 19, email: 'mary.doe@email.com' }, { id: 3, name: 'Jim Doe', age: 16, email: 'jim.doe@email.com' }, { id: 4, name: 'Martha Doe', age: 25, email: 'martha.doe@email.com' }]"></DynamicTable>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import DynamicTable from '@/components/dynamic-table.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld,
    DynamicTable
  }
}
</script>
