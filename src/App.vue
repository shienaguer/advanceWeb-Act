
<script setup>
import { ref } from 'vue';

const inputText = ref('hello')
const car = ref('')

</script>
<template>
  <div  class="p-3 mb-2 bg-danger-subtle text">
    <div class="mx-auto p-2" style="width: 800px; ">
  <h2>Description Of Car</h2>
  <div  class="p-3 mb-2 bg-black text-white">
    <select v-model="car"  class="form-select form-select-lg mb-3" aria-label="Large select example">
     
        <option value="car1">Toyota Camry</option>
        <option value="car2">Ford Mustang</option>
        <option value="car3">Honda Civic</option>
        <option value="car4">Chevrolet Silverado</option>
        <option value="car5">Tesla Model 3</option>
        <option value="car6">BMW X5</option>

       
    </select>
    <p v-if="car == 'car1'">
      <h5>Toyota Camry</h5>
    <p>Year: 2023</p>
    <p>Make: Toyota</p>
    <p>Model: Camry</p>
    <p>Body Style: Sedan</p>
    <p>Engine: 2.5L Inline-4</p>
    <p>Price: $25,000</p>
    </p>
    <p v-if="car == 'car2'">
      <h5>Ford Mustang</h5>
    <p>Year: 2023</p>
    <p>Make: Ford</p>
    <p>Model: Mustang</p>
    <p>Body Style: Coupe</p>
    <p>Engine: 5.0L V8</p>
    <p>Price: $45,000</p>
</p>
<p v-if="car == 'car3'">
  <h5>Honda Civic</h5>
    <p>Year: 2023</p>
    <p>Make: Honda</p>
    <p>Model: Civic</p>
    <p>Body Style: Compact Sedan</p>
    <p>Engine: 2.0L Inline-4</p>
    <p>Price: $22,000</p>
</p>
<p v-if="car == 'car4'">
  <h5>Chevrolet Silverado</h5>
    <p>Year: 2023</p>
    <p>Make: Chevrolet</p>
    <p>Model: Silverado</p>
    <p>Body Style: Pickup Truck</p>
    <p>Engine: 5.3L V8</p>
    <p>Price: $35,000</p>
</p>
<p v-if="car == 'car5'">
  <h5>Tesla Model 3</h5>
    <p>Year: 2023</p>
    <p>Make: Tesla</p>
    <p>Model: Model 3</p>
    <p>Body Style: Electric Sedan</p>
    <p>Range: 350 miles</p>
    <p>Price: $42,000</p>
</p>
<p v-if="car == 'car6'">
  <h5>BMW X5</h5>
    <p>Year: 2023</p>
    <p>Make: BMW</p>
    <p>Model: X5</p>
    <p>Body Style: SUV</p>
    <p>Engine: 3.0L Inline-6</p>
    <p>Price: $60,000</p>
</p>
</div>
</div>
</div>
    <!-- <p v-else>3</p> -->
</template>