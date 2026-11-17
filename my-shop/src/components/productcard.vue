<template>
<div class="product_card">
<img  :src="image" alt="name" class="product-image"> 
<h2>{{ name }}</h2>
<p>{{ description }}</p>
<p class="price">{{ price}} грн</p>
<button class="by-button">Купити</button>
</div>
</template>

<script setup>
/* eslint-disable no-undef */
defineProps({
  name: String,
  description: String,
  price: Number,
  image: String
})
</script>

<style scoped>
.product_card {
  background-color: #ffffff;
  border-radius: 16px;
  padding: 20px;
  width: 280px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
.product-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 12px;
  margin-bottom: 16px;
}

.product_card h2 {
  font-size: 20px;
  color: #2c3e50;
  margin: 0 0 8px 0;
  font-weight: 600;
}

.product_card p {
  font-size: 14px;
  color: #7f8c8d;
  margin: 0 0 16px 0;
}

.price {
  font-size: 22px;
  font-weight: 700;
  color: #8b0000; 
  margin: 0 0 16px 0;
}

.by-button {
  background-color: #a91d22; 
  color: white;
  border: none;
  border-radius: 8px;
  padding: 10px 24px;
  font-size: 16px;
  font-weight: 600;
  cursor: pointer;
  width: 100%;
  transition: background-color 0.2s ease;
}

.by-button:hover {
  background-color: #801217; 
}
</style>