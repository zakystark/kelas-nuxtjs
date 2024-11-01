<script lang="ts" setup>
import { products } from '~/commons/data';

const route = useRoute()
const paramsId = route.params.id

const productById =products.filter(item => item.id === Number(paramsId))

</script>


<template>
    <div class="flex flex-row items-start gap-4">
        <img
        :src="productById[0].image"
        alt="sepatu cowok"
        >

        <div class="flex flex-col gap-2">
            <h1 class="text-2x1">{{ productById[0].title }}</h1>
            <p class="text-lg">{{ productById[0].stock }}</p>
            <p class="text-lg">{{ productById[0].description }}</p>

            <div class="flex flex-row gap-2">
                <button class="min-w-[120px] bg-yellow-300 text-white p-2 rounded-lg">
                    Tambah keranjang
                </button>

                <button class="min-w-[120px] bg-yellow-300 text-white p-2 rounded-lg">
                 Beli
                </button>
            </div>
        </div>
    </div>
</template>