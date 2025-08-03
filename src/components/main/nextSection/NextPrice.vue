<template>
  <main>
    <section>
      <div class="border absolute rounded-[10px] mt-[-360px] ml-[880px] z-10 p-[20px] border-[#1ABA1A]">
        <div>
          <p class="font-[700] text-[16px] text-[#000000] mb-[35px] leading-[24px]">Order Summary</p>
          <div class="flex gap-[157px] mb-[12px]">
            <p class="font-[400] text-[#666666] text-[14px] leading-[21px]">Sub Total:</p>
            <p class="font-[700] text-[14px] text-[#000000] leading-[21px]">$1,000.00</p>
          </div>
          <div class="w-[50px mb-[15px] h-[0.5px] opacity-50 bg-[#666666]"></div>
          <div class="flex gap-[116px] mb-[12px]">
            <p class="font-[400] text-[#666666] text-[14px] leading-[21px]">Shpping estimate:</p>
            <p class="font-[700] text-[14px]  text-[#000000] leading-[21px]">$600.00</p>
          </div>
          <div class="w-[50px mb-[15px] h-[0.5px] opacity-50 bg-[#666666]"></div>
          <div class="flex gap-[150px] mb-[12px]">
            <p class="font-[400] text-[#666666] text-[14px] leading-[21px]">Tax estimate:</p>
            <p class="font-[700] text-[14px] text-[#000000] leading-[21px]">$137.00</p>
          </div>
          <div class="w-[50px mb-[15px] opacity-50 h-[0.5px] bg-[#666666]"></div>
          <div class="flex gap-[120px]">
            <p class="uppercase font-[700] text-[14px] text-[#000000] leading-[21px]">Order total:</p>
            <p class="font-[700] text-[14px] text-[#000000] leading-[21px]">{{formatted}}</p>
          </div>
          <button class="uppercase ml-[60px] py-[15px] px-[40px] mt-[30px] rounded-[10px] text-[#FFFFFF] bg-[#1ABA1A]">checkout</button>
        </div>
      </div>
    </section>
  </main>
</template>
<script setup>
let totalMoney = 1737
let formatted = `$${totalMoney.toLocaleString(undefined, { minimumFractionDigits: 2, maximumFractionDigits: 2 })}`
</script>