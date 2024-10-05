<script setup>
import { ref } from "vue";
import categories from "./categories.vue";
const mobileDatabase = ref([
  {
    m_name: "Galaxy Note10+ 5G",
    imgUrl: "src/images/6d2x.png",
    desc: "/Samsung",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Galaxy S10",
    imgUrl: "src/images/7beyond1lte.png",
    desc: "/Samsung",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "A73 5G",
    imgUrl: "src/images/8a73xq.png",
    desc: "/Samsung",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "A52 4g",
    imgUrl: "src/images/9a52q.png",
    desc: "/Samsung",
    price: 2800,
    quantity: 1,
  },



  {
    m_name: "Realme 5s",
    imgUrl: "src/images/11r5x.png",
    desc: "/realme",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Realme 2 Pro",
    imgUrl: "src/images/12r2p.png",
    desc: "/realme",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Realme 6 Pro",
    imgUrl: "src/images/13RMX2061.png",
    desc: "/realme",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Realme 5 Pro",
    desc: "/realme",
    imgUrl: "src/images/14RMX1971.png",
    price: 2800,
    quantity: 1,
  },



  {
    m_name: "OnePlus Nord",
    imgUrl: "src/images/15avicii.png",
    desc: "/OnePlus",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "OnePlus 5",
    imgUrl: "src/images/16dre.png",
    desc: "/OnePlus",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "OnePlus Nord N200",
    imgUrl: "src/images/17dumpling.png",
    desc: "/OnePlus",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "OnePlus 5T",
    imgUrl: "src/images/18fajita.png",
    desc: "/OnePlus",
    price: 2800,
    quantity: 1,
  },


  {
    m_name: "Pixel  5a",
    imgUrl: "src/images/21barbet.png",
    desc: "/Pixel",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Pixel  3",
    imgUrl: "src/images/22blueline.png",
    desc: "/Pixel",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Pixel  3A XL",
    imgUrl: "src/images/23bonito.png",
    desc: "/Pixel",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Pixel  XL",
    imgUrl: "src/images/24marlin.png",
    desc: "/Pixel",
    price: 2800,
    quantity: 1,
  },



  {
    m_name: "Moto Z2 Play",
    imgUrl: "src/images/25albus.png",
    desc: "/Motorola",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Moto G6",
    imgUrl: "src/images/26ali.png",
    desc: "/Motorola",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Moto Z3 Play",
    imgUrl: "src/images/27beckham.png",
    desc: "/Motorola",
    price: 2800,
    quantity: 1,
  },
  {
    m_name: "Moto One Power",
    imgUrl: "src/images/28chef.png",
    desc: "/Motorola",
    price: 2800,
    quantity: 1,
  },
]);
</script>

<template>
  <categories :mobileDatabase="mobileDatabase" />
</template>
