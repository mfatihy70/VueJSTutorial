<!-- <script>
export default{
  data(){
    return{
      name: 'John Doe',
      status: 'active',
      tasks: ['Task 1', 'Task 2', 'Task 3'],
      link: 'http://google.com'
    }
  }
}
</script>


<template>
  <h1>{{ name }}</h1>
  <p v-if="status">User is active</p>
  <p v-else-if="status === 'inactive'">User is inactive</p>
  <p v-else>User is inactive</p>
  <br>
  <h3>Tasks:</h3>
  <ul>
    <li v-for="task in tasks" :key="task">{{ task }}</li>
  </ul>
  <br>
  <a :href="link">Click for link</a>

  <button v-on=""></button>
</template> -->

<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>