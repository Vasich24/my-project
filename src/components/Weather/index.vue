<template>
  <div>
    <select>
      <option>{{ goroda[0] }}</option>
      <option>{{ goroda[1] }}</option>
      <option>{{ goroda[2] }}</option>
    </select>
    <span> сьогодні о 9:00</span>
    <div class="first">
      <div class="second">
        <img
          class="cartinka"
          src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTtK8lBxG07jD2EUFzhdabN-k5QKPBN2VG9hw&usqp=CAU"
        />
        <span style="font-size: 40px">+12°C</span>
      </div>
      <div class="thrid">
        <span>вологість: 90%</span><br />
        <span>тиск: 780мм</span><br />
        <span>вітер: 0 м/с</span><br />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Weather",
  props: {
    goroda: {
      type: Array,
      default: () => ["Ужгород", "Київ", "Львів"],
    },
  },
};
</script>

<style lang="css" scoped>
.cartinka {
  width: 50px;
}
</style>