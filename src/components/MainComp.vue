<template>
  <main>
    <SecOne />
    <SecTwo />
    <SecThree />
  </main>
</template>

<script>
import SecOne from "./sections/SecOne.vue";
import SecTwo from "./sections/SecTwo.vue";
import SecThree from "./sections/SecThree.vue";
export default {
    components: { SecOne, SecTwo, SecThree }
}
</script>

<style lang="scss" scoped>

</style>