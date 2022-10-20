<template>
  <div></div>
</template>

<script>

import {goods} from "@/api";
export default {
  created() {
    this.getdata();
  },
  methods: {
    async getdata() {
      let res = await goods();
      console.log(res.data);
    },
  },
};
</script>

<style lang="scss" scoped>
</style>