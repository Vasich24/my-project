<template>
  <div>
    <table border="2px solid">
      <tr>
        <td>Назва продукту</td>
        <td>{{ bludo }}</td>
      </tr>
      <tr>
        <td>Вартість</td>
        <td>{{ vartist + "грн" }}</td>
      </tr>
      <tr>
        <td>ПДВ</td>
        <td>{{ pdv + "%" }}</td>
      </tr>
      <tr>
        <td>До оплати</td>
        <td>{{ suma + "грн" }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "TableAl",
  props: {
    bludo: {
      type: String,
      default: "Сир",
    },
    vartist: {
      type: Number,
      default: 100,
    },
    pdv: {
      type: Number,
      default: 5,
    },
  },
  computed: {
    suma() {
      return this.vartist + (this.vartist * this.pdv) / 100;
    },
  },
};
</script>

<style lang="css" scoped>
</style>