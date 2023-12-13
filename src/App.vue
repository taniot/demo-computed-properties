<script>
export default {
  name: 'DefaultTemplate',

  data() {
    return {
      text: 'Template VueJS',
      firstName: 'Gaetano',
      middleName: '',
      lastName: 'Frascolla',
      age: 40,
    };
  },
  methods: {
    // getFullName() {
    //   console.log('sono stato invocato');
    //   return `${this.firstName} ${this.middleName} ${this.lastName}`;
    // },
  },
  computed: {
    getFullName() {
      console.log('sono stato invocato');
      return `${this.firstName} ${this.middleName} ${this.lastName}`;
    },
  },
};
</script>

<template>
  <h1>
    {{ getFullName }}
  </h1>

  <div>
    <label>FirstName</label>
    <input type="text" v-model="firstName" />
    <label>middleName</label>
    <input type="text" v-model="middleName" />
    <label>lastName</label>
    <input type="text" v-model="lastName" />
    <label>age</label>
    <input type="number" v-model="age" />
  </div>
</template>

<style scoped lang="scss"></style>
