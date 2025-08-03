<template>
  <main>
    <section>
      <div class="bg-[#FAFAFA] rounded-[10px] mr-[340px]">
        <div class="m-4  flex items-start justify-between">
          <div class="flex gap-[20px]">
            <div>
              <div class="bg-[#000000] mt-[20px] px-2 py-1 absolute rounded-[7px]">
                <p class="font-[500] text-[12px] text-[#FFFFFF]">NEW</p>
              </div>
              <img class="w-[270px] h-[320px]" src="../../../assets/images/ipad.png" alt="iPad">
            </div>
            <div class="mt-10">
              <p class="ml-[70px]">({{product}})</p>
              <p class="font-[700] text-[16px] mt-[8px] text-[#000000] leading-[17px]">aPod Pro Tablet 2023 LTE + Wifi, GPS Cellular 12.9 Inch, 512GB</p>
              <p class="font-[600] text-[18px] text-[#000000] leading-[22px] mt-[16px] mb-[20px]">{{changePrice}}</p>
              <div class="flex items-center py-[5px] px-[20px] gap-[20px] absolute rounded-[10px] border border-[#999999]">
                <img @click="ChangeRemove" class="cursor-pointer" src="../../../assets/images/Minus.svg" alt="minus" width="11px" height="13px">
                <p class="font-[500]">{{add}}</p>
                <img @click="ChangeAdd" class="cursor-pointer" src="../../../assets/images/Plus.svg" alt="Plus" width="11px" height="13px">
              </div>
              <div class="bg-[#E2E4EB] px-[15px] mt-[58px] rounded-[9px] py-[2px] absolute">
                <p class="text-[#000000] text-[14px] font-[500]">$2.98 SHIPPING</p>
              </div>
              <div class="flex mt-[120px] items-center gap-[10px]">
                <img class="mt-[2px]" src="../../../assets/images/True.svg" alt="True">
                <p>In stock</p>
              </div>
            </div>
          </div>
          <div class="flex m-4 gap-[10px]">
            <div class="w-[50px] h-[50px] bg-[#E2E4EB] rounded-[50px]"></div>
            <div class="w-[50px] h-[50px] bg-[#FF000011] rounded-[50px]"></div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>
<script setup>
import { ref } from "vue";

let product = 15
let basePrice = 979

let add = ref(1)

let changePrice = ref(`$${basePrice.toFixed(2)}`)

function ChangeAdd() {
  add.value++
  let number = basePrice * add.value
  changePrice.value = `$${number.toFixed(2)}`
  product--
  if (product < 0){
    alert("mahsulot qolmadi")
  }
}

function ChangeRemove() {
  if (add.value > 1) {
    add.value--
    let number = basePrice * add.value
    changePrice.value = `$${number.toFixed(2)}`
    product++

  }
}
</script>