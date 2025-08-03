<template>
  <div class="bg-[#FFFFFF] w-[1250px] my-[16px] pt-[30px] pb-[30px] rounded-[10px] px-[25px] mx-auto">
    <div>
      <sectionOne></sectionOne>
      <sectionTwo></sectionTwo>
      <sectionThree></sectionThree>
    </div>
    <sectionPrice></sectionPrice>
  </div>
</template>

<script setup>
import sectionOne from "./nextSection/nextProtuctOne.vue"
import sectionTwo from "./nextSection/nextProtuctTwo.vue"
import sectionThree from "./nextSection/NextProductThree.vue"
import sectionPrice from "./nextSection/NextPrice.vue"
</script>