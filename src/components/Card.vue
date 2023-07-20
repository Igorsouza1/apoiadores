<template>
    <div class="card">
        <img :src="image" alt="Card image" class="card-image">
        <div class="card-content">
        <h2 class="card-name">{{ name }}</h2>
        </div>
    </div>
  </template>
  
  <script>

  
  export default {
    name: 'CardComponent',
    props: {
        image: String,
        name: String
    }
  }
  </script>

<style scoped>
.card {
  border: 1px solid #ccc;
  border-radius: 10px;
  width: 300px;
  overflow: hidden;
  box-shadow: 0px 4px 6px rgba(0,0,0,0.1);
  margin: 30px;
  cursor: pointer;
}

.card-image {
  width: 100%;
  height: 200px;
  object-fit: contain;
  padding: 10px;
}

.card-content {
  padding: 15px;
}

.card-name {
  margin: 0;
  margin-bottom: 10px;
  font-size: 20px;
  line-height: 1.2;
  text-align: center;
}
</style>
  