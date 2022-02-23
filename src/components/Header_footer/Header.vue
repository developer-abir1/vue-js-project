<template>
  <div>
    <p>fastName: {{ fastName }}</p>
    <p>lasttName: {{ lastName }}</p>
    <p>Client Age : {{ age }}</p>
    <button @click="updateName">Update Name</button>
  </div>
</template>

<script>
export default {
  props: {
    fastName: String,
    lastName: String,
    age: Number,
  },
  methods: {
    updateName() {
      this.$emit("updateValue", "Kalifaae e");
    },
  },
};
</script>

<style lang="scss" scoped></style>
