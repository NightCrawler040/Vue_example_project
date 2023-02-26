<script setup>
import {ref} from "vue";

const _products = ref([
  {
    id:1,
    title:"Iphone 12",
    price:1000,
    img:"https://www.technodom.kz/_next/image?url=https%3A%2F%2Fapi.technodom.kz%2Ff3%2Fapi%2Fv1%2Fimages%2F800%2F800%2F228613_1.jpg&w=3840&q=85"
  },
  {
    id:2,
    title:"Iphone 13",
    price:1200,
    img: 'https://www.technodom.kz/_next/image?url=https%3A%2F%2Fapi.technodom.kz%2Ff3%2Fapi%2Fv1%2Fimages%2F800%2F800%2F252987_1.jpg&w=3840&q=85'
  },
  {
    id:1,
    title:"Iphone 14",
    price:1400,
    img: 'https://www.technodom.kz/_next/image?url=https%3A%2F%2Fapi.technodom.kz%2Ff3%2Fapi%2Fv1%2Fimages%2F800%2F800%2F265281_1.jpg&w=3840&q=85'
  }
]);
</script>

<template>
  <div>
    <div v-for="product in _products" :key="product.id">
      <img :alt="product.title" :src="product.img" >
      <p>{{product.title}}</p>
      <p>{{product.price}}</p>
    </div>
  </div>
</template>





















