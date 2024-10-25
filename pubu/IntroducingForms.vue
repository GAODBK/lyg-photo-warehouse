<script setup>
const props = defineProps(["formDisplayContent"]);
const emit = defineEmits(["colseFrom", "addData"]);

const closeTheIntroductionForm = () => {
  emit("colseFrom");
};

const dataUsageAddition = (value) => {
  console.log(value);
  emit("addData", value);
};
</script>

<template>
  <div>
    <div class="blackInterface">
      <div class="blackWindow">
        <div class="btn" @click="closeTheIntroductionForm"></div>
        <div class="left">
          <img :src="formDisplayContent.url" />
        </div>

        <div style="float: right; max-width: 780px">
          <h4>{{ formDisplayContent.text }}</h4>

          <p>
            价格：<span style="color: red; font-size: 20px">
              ￥{{ formDisplayContent.price }}</span
            >
          </p>
          <p>菜品名称：{{ formDisplayContent.num }}</p>
          <p>已售: 65</p>
          <p>
            规格：
            <span style="color: red; border: 1px solid #ff0000">357g</span>
          </p>
          <!-- <p>
            数量：
            <input type="button" value="-" />
            <input type="text" style="width: 20px" value="1" />
            <input type="button" value="+" />
          </p> -->
          <input
            type="submit"
            @click="dataUsageAddition(formDisplayContent)"
            value="立即订购"
            style="width: 100px; height: 40px; background: #ff0000; border: 0"
          />
          <p>温馨提示:不满意就退款 电话订购: 400-9700-910</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.btn {
  position: relative;
  width: 40px;
  height: 40px;
  cursor: pointer;
}

.left {
  float: left;
  margin: 18px 0 0 10px;
  width: 400px;
}

.left img {
  width: 100%;
  height: 600px;
  object-fit: cover;
  border-radius: 5px;
}

img {
  max-width: 400px;
  margin: auto 0;
}
.btn::before,
.btn::after {
  content: "";
  position: absolute;
  top: 50%;
  left: 50%;
  width: 30px;
  height: 2px;
  background-color: #000;
  transform-origin: center;
}

.btn::before {
  transform: translate(-50%, -50%) rotate(45deg);
}

.btn::after {
  transform: translate(-50%, -50%) rotate(-45deg);
}

.btn:hover::before,
.btn:hover::after {
  background-color: #ff0000;
}

.blackInterface {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.7);
  /* 半透明黑色背景 */
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;
  /* 确保在顶层 */
  animation: 2.5s cubic-bezier(0.25, 1, 0.3, 1) animationEffects both;
}

.btn:focus .blackInterface {
  animation: 2.5s cubic-bezier(0.25, 1, 0.3, 1) tuichu both;
}

.blackWindow {
  background-color: rgb(245, 245, 251);
  font-size: 24px;

  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  border-radius: 5px;
  padding: 20px;
  margin-top: 20px;
  text-align: center;
  position: relative;

  width: 1200px;
  height: 700px;
  animation: 2.5s cubic-bezier(0.25, 0.6, 0.3, 1) animationEffects both;
}

@keyframes animationEffects {
  from {
    clip-path: circle(0%);
  }

  to {
    clip-path: circle(150% at top left);
  }
}
</style>
