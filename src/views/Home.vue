<template>
  <div class="home">
 <h1>Home</h1>
 <p ref="p">My name is {{ name }} and I am {{ age }} years.</p>
  </div>
  <button @click="handleClick">Click Me!</button>
</template>

<script>
import { ref } from '@vue/reactivity'

export default {
  name: 'Home',
  setup() {
    const name = ref('Kim')
    const age = ref(300)

    const p = ref(null)

  const handleClick = () => {
    console.log(p, p.value)
    p.value.classList.add('param')
    p.value.textContent = 'Hello Kim Ninja'
   name.value =' Nigel'
   age.value = 29
  }

 return{name, age, handleClick, p}
  }
 
}
</script>
