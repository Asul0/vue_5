<template>
    <div class="product-details">
      <h1>{{ product.name }}</h1>
      <p class="price">{{ formattedPrice }}</p>
      <p class="availability">{{ product.available ? 'Available' : 'Out of stock' }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ProductDetails',
    data() {
      return {
        product: {
          name: 'Example Product',
          price: 99.99,
          available: true
        }
      };
    },
    computed: {
      formattedPrice() {
        return `$${this.product.price.toFixed(2)}`;
      }
    }
  };
  </script>
  
  <style scoped>
  .product-details {
    text-align: center;
    margin-top: 20px;
    font-family: Arial, sans-serif;
    background-color: #f9f9f9;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .product-details h1 {
    font-size: 2.5em;
    color: #333;
    margin-bottom: 10px;
  }
  
  .product-details .price {
    font-size: 2em;
    color: #4CAF50;
    margin: 10px 0;
  }
  
  .product-details .availability {
    font-size: 1.5em;
    color: #f44336;
  }
  
  .product-details .availability.available {
    color: #4CAF50;
  }
  </style>
  