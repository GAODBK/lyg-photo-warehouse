<script setup>
import {ref} from "vue";
import ShopByCategory from './ShopByCategory.vue'

const foodData = ref([
  {
    f_name: "绿芦笋",
    price: 23,

    imgUrl: 'src/images/1green-asparag.jpg',
    desc: ["蔬菜"]
  },
  {
    f_name: "卷心菜",
    price: 23,

    imgUrl: 'src/images/2kohlrabi.jpg',
    desc: ["蔬菜", "苤", "德国萝卜", "野白菜"]
  },
  {
    f_name: "大蒜",
    price: 23,

    imgUrl: 'src/images/3garlic.jpg',
    desc: ["蔬菜", "香料"]
  },
  {
    f_name: "生菜叶",
    price: 23,

    imgUrl: 'src/images/4green.jpg',
    desc: ["蔬菜", "收成", "叶子"]
  },
  {
    f_name: "番茄 ",
    price: 23,

    imgUrl: 'src/images/5tomatoe.jpg',
    desc: ["蔬菜", "罗勒", "意大利美食", "有机的"]
  },
  {
    f_name: "西葫芦",
    price: 23,

    imgUrl: 'src/images/7zucchinis.jpg',
    desc: ["蔬菜", "新鲜的", "黄色"]
  },
  {
    f_name: "南瓜",
    price: 23,

    imgUrl: 'src/images/8pumpkins.jpg',
    desc: ["蔬菜", "装饰葫芦科", "收成", "生产"]
  },

  {
    f_name: "土豆",
    price: 23,

    imgUrl: 'src/images/6potatoe.jpg',
    desc: ["蔬菜", "豆芽", "收成", "新鲜的"]
  },
  {
    f_name: "布鲁塞尔豆芽",
    price: 23,

    imgUrl: 'src/images/9brussels-sprouts.jpg',
    desc: ["蔬菜", "豆芽", "收成", "新鲜的"]
  },


  {
    f_name: "黑莓",
    price: 23,

    imgUrl: 'src/images/11berry.jpg',
    desc: ["水果", "浆果", "维生素"]
  },
  {
    f_name: "蓝莓",
    price: 23,

    imgUrl: 'src/images/12blueberries.jpg',
    desc: ["水果", "营养", "健康", "新鲜的"]
  },
  {
    f_name: "草莓",
    price: 23,

    imgUrl: 'src/images/13strawberries.jpg',
    desc: ["水果", "健康", "维生素"]
  },
  {
    f_name: "山莓",
    price: 23,

    imgUrl: 'src/images/14fruits.jpg',
    desc: ["水果", "浆果", "成熟", "新鲜的"]
  },
  {
    f_name: "橙子",
    price: 23,

    imgUrl: 'src/images/16oranges.jpg',
    desc: ["水果", "收成", "新鲜的"]
  },
  {
    f_name: "桃子",
    price: 23,

    imgUrl: 'src/images/15peache.jpg',
    desc: ["水果", "新鲜的", "维生素"]
  },
  {
    f_name: "山莓",
    price: 23,

    imgUrl: 'src/images/17raspberries.jpg',
    desc: ["水果", "新鲜的", "健康", "营养"]
  },


  {
    f_name: "pork food",
    price: 23,

    imgUrl: 'src/images/21steamed-pork.jpg',
    desc: ["肉制品", "pork"]
  },
  {
    f_name: "香肠",
    price: 23,

    imgUrl: 'src/images/23sausages.jpg',
    desc: ["肉制品", "烧烤", "炙烤"]
  },
  {
    f_name: "牛排",
    price: 23,

    imgUrl: 'src/images/24meat.jpg',
    desc: ["肉制品", "烤羊肉", "蛋白质"]
  },
  {
    f_name: "火腿",
    price: 23,

    imgUrl: 'src/images/22ham.jpg',
    desc: ["肉制品", "肉", "帕塔内格拉"]
  },
  {
    f_name: "鸭脯",
    price: 23,

    imgUrl: 'src/images/25meat.jpg',
    desc: ["肉制品", "生的", "可口"]
  },
  {
    f_name: "鸡肉",
    price: 23,

    imgUrl: 'src/images/26chicken.jpg',
    desc: ["肉制品", "烤箱食品", "一顿饭"]
  },


  {
    f_name: "苹果汁",
    price: 23,

    imgUrl: 'src/images/31punch.jpg',
    desc: ["饮料", "烤箱食品", "一顿饭"]
  },
  {
    f_name: "热葡萄酒",
    price: 23,

    imgUrl: 'src/images/32mulled-wine.jpg',
    desc: ["饮料"]
  },
  {
    f_name: "桔子汁",
    price: 23,

    imgUrl: 'src/images/33orange-juice.jpg',
    desc: ["饮料"]
  },
  {
    f_name: "葡萄柚汁",
    price: 23,

    imgUrl: 'src/images/34cocktails.jpg',
    desc: ["饮料"]
  },
  {
    f_name: "醋栗汁汽水",
    price: 23,

    imgUrl: 'src/images/35drink.jpg',
    desc: ["饮料"]
  }
])
</script>

<template>
  <ShopByCategory :foodData="foodData"/>
</template>