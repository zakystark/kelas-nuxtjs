<script lang="ts" setup>
    const products =[
        {
            id:'1',
            image: 'https://images.tokopedia.net/img/cache/100-square/VqbcmM/2022/1/16/1abf9771-e4c9-47c8-b77a-95a05fc4bb34.jpg.webp?ect=4g',
            title: 'sepatu cowok',
            price: 'RP5.000',
        },
        {
            id:'2',
            image: 'https://images.tokopedia.net/img/cache/100-square/VqbcmM/2022/1/16/bc8109af-9382-4c51-8ca0-e042687c8fe1.jpg.webp?ect=4g',
            title: 'sepatu cewek',
            price: 'RP5.000',
        }

    ]
</script>
<template>
    <div class="flex flex-col gap-4">
        <h1 class="text-lg font-semibold">produk barang</h1>
            <ul class="flex flex-row flex-wrap gap-2">
                <li class="p-2 rounded-md w-[150px] h-auto shadow-lg"
                v-for="(products, index) in products"
                :key="index"
                >
            <div class="flex flex-col gap-1">
                <img
                    :src="products.image"
                    alt="gambar produk"
                    >
                    <h3 class="text-xs">{{ products.title }}</h3>
                    <h3 class="text-xs font-bold">{{ products.price }}</h3>

            </div>

                </li>
            </ul>
        
    </div>
</template>