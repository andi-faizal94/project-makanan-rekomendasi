<template>
  <div>
    <isi />
    {{hasilSearch}}
  </div>
</template>
<script>
import isi from "@/components/isi.vue";
export default {
  components: {
    isi
  },
  data: () => {},
  methods: {
    hasilSearch() {
      this.$store.commit("getDataMieAyam", this.mieAyam);
    }
  }
};
</script>
<style lang="stylus"></style>