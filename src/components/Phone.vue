<template>
    <div class="lg:py-10 text-center mt-16 relative">

        <div class="absolute  w-[100%] flex items-center justify-center h-[100%] z-[-1] rounded-full">
            <div class="bg-white/10 rounded-full h-[90vh] blur-3xl w-[70%]">

            </div>
        </div>
        <h2 class="text-white text-[32px] font-[700]">
            Powerful Features for Smarter Trading
        </h2>

        <div class="grid grid-cols-1 lg:grid-cols-3 gap-10 w-[80%] mx-auto mt-16">
            <div class="flex flex-col justify-evenly  h-full gap-10 lg:gap-0">
                <div v-for="i in col1" class="flex flex-col gap-3 text-left group">
                    <div class="relative w-[42px] h-[42px]">
                        <img :src="i.img1" alt=""
                            class=" absolute inset-0 w-full h-full group-hover:opacity-0 transition-opacity">
                        <img :src="i.img" alt=""
                            class="absolute inset-0 w-full h-full opacity-0 group-hover:opacity-100 transition-opacity">
                    </div>

                    <h4 class="transition-all duration-150 text-[19.2px] font-[700] text-white group-hover:text-[#23BDB9]">
                        {{ i.title }}
                    </h4>
                    <p class="transition-all duration-150 font-[600] text-[16px] text-white max-w-52 group-hover:text-[#23BDB9]">
                        {{ i.description }}
                    </p>
                </div>

            </div>
            <div class="flex justify-center ">
                <img src="/src/assets/img/phone.png" alt="" class="w-96">
            </div>
            <div class="flex flex-col justify-evenly  h-full gap-10 lg:gap-0">
                <div v-for="i in col2" class="flex flex-col gap-3 text-left group">
                    <div class="relative w-[42px] h-[42px]">
                        <img :src="i.img1" alt=""
                            class="absolute inset-0 w-full h-full group-hover:opacity-0 transition-opacity">
                        <img :src="i.img" alt=""
                            class="absolute inset-0 w-full h-full opacity-0 group-hover:opacity-100 transition-opacity">
                    </div>

                    <h4 class="transition-all duration-150 text-[19.2px] font-[700] text-white group-hover:text-[#23BDB9]">
                        {{ i.title }}
                    </h4>
                    <p class=" transition-all duration-150 font-[600] text-[16px] text-white max-w-52 group-hover:text-[#23BDB9]">
                        {{ i.description }}
                    </p>
                </div>

            </div>
        </div>
    </div>
</template>

<script setup>

import ai from '@/assets/svg/phone/ai.svg'
import graph from '@/assets/svg/phone/graph.svg'
import shop from '@/assets/svg/phone/shop.svg'
import Group from '@/assets/svg/phone/Group.svg'
import handshake from '@/assets/svg/phone/handshake.svg'
import strategy from '@/assets/svg/phone/startegy.svg'
import ai_white from '@/assets/svg/phone/ai_white.svg'
import graph_white from '@/assets/svg/phone/graph_white.svg'
import shop_white from '@/assets/svg/phone/shop_white.svg'
import Group_white from '@/assets/svg/phone/Group_white.svg'
import handshake_white from '@/assets/svg/phone/handshake_white.svg'
import strategy_white from '@/assets/svg/phone/startegy_white.svg'
// import strategy from '@/assets/svg/phone/strategy.svg'

const col1 = [
    {
        title: '100% Automated Trading',
        description: 'Let our system handle trades for you effortlessly.',
        img: Group,
        img1: Group_white
    },
    {
        title: 'Multiple Effective Tested Strategies',
        description: 'Maximize profits with high-accuracy strategies.',
        img: ai,
        img1: ai_white
    },
    {
        title: 'Trade Major Indices',
        description: 'Let our system handle trades for you effortlessly.',
        img: graph,
        img1: graph_white
    },
]

const col2 = [
    {
        title: 'Wide Market Coverage',
        description: ' Supports F&O, MCX, NSE, BSE & ETFs.',
        img: shop,
        img1: shop_white
    },
    {
        title: 'Custom Strategy Support',
        description: 'Create & automate your own trading strategies.',
        img: strategy,
        img1: strategy_white
    },
    {
        title: 'Multiple Broker Integration',
        description: 'Connect seamlessly with your preferred broker.',
        img: handshake,
        img1: handshake_white
    },
]

</script>

<style lang="scss" scoped></style>