<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
  </div>

  
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

.button {
  font-family: kanit;
  color: #ffffff;
  background-color: #55ab41;
  margin: 5px;
  padding: 10px;
  width: 40%;
  border-style: none;
  border-radius: 10px;
}

.content {
  background-repeat: no-repeat;
  background-size: cover;
  margin: 10px;
  padding: 0;
  font-family: kanit;
}

.box {
  text-align: center;
  background-color: #ffffff;
  padding: 5%;
  margin: 5%; 
  border: 2px solid #ffffff;
  border-radius: 10px;
  box-shadow: 0 4px 4px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

.box-1, .box-2 {
  width: 100%; 
  box-sizing: border-box;
  padding: 5px;
}

textarea {
  width: 80%;
  height: 60px;
  padding: 10px;
  border: 2px solid #3d3d33;
  border-radius: 5px;
}
.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
