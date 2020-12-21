<template>
  <div id="persons">
    <ul>
      <li v-for="(person,index) in persons" :key="person.id" v-on:click="person.show = !person.show">
        <h2>{{ [index+1] + '. ' + person.name }}</h2>
        <h3 v-show="person.show">{{ person.speciality }}</h3>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  data(){
    return{
      persons: [
        {name: 'Roshan', speciality: 'Developer', show: false},
        {name: 'Hari', speciality: 'Designer', show: false},
        {name: 'Sita', speciality: 'Teacher', show: false},
        {name: 'Ram', speciality: 'Doctor', show: false},
        {name: 'Mahesh', speciality: 'Pilot', show: false},
        {name: 'Gopal', speciality: 'Scientist', show: false}
      ]
    }
  }
}
</script>
<style scoped>
#persons{
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
  box-sizing: border-box;
}
ul{
  display: flex;
  flex-wrap: wrap;
  list-style-type: none;
  padding: 0;
}
li{
  flex-grow: 1;
  flex-basis: 300px;
  text-align: center;
  padding: 30px;
  border: 1px solid #222;
  margin: 10px;
}
</style>