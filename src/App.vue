<script setup>
import { ref } from 'vue'
  const count = ref(0);

  const addToCount = () =>{
    
    count.value = count.value + 1
  }
  const subtractFromCount = () => {
    
    count.value = count.value - 1
  }

</script>


<template>
  <main>
    <div>
      <h1>The Vue Counter</h1>
      <p>Developed by Nasim Qureshi</p>
      <h1>
        <span>{{ count }}</span>
      </h1>
      <button @click=addToCount()>+</button>
      <button @click=subtractFromCount()>-</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aliceblue;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
}
div {
  text-align: center;
}
</style>