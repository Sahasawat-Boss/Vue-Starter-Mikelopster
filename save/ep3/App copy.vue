<script setup>
import { ref, computed } from 'vue'
const priceUSD = ref(0)
const exchangeRate = 35

const priceTHB = computed({
    get: () => priceUSD.value * exchangeRate,
    // compute get
    // compute update will use set
    set: (newValue) => {
        priceUSD.value = (newValue / exchangeRate)
    }
})
</script>

<template>
    <div>
        Price in USD <input type="number" v-model="priceUSD">
        Price in THB <input type="number" v-model="priceTHB">
        <p>Price in USD: ${{ priceUSD }}</p>
        <p>Price in THB: {{ priceTHB }}฿</p>
    </div>
</template>