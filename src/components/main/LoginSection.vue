<template>
  <main>
    <section>
      <div class="w-[1250px] my-[16px] pt-[68px] pb-[47px] rounded-[10px] px-[120px] mx-auto bg-[#FFFFFF]">
        <div class="flex items-center justify-between">
          <img src="../../assets/images/LoginImages.png" alt="LoginImage" width="403" height="328" />
          <div>
            <p class="font-[700] text-[28px] leading-[33px] text-[#1ABA1A] mb-[10px]">Welcome Back</p>
            <p class="font-[500] text-[14px] text-[#999999] leading-[23px] tracking-[2.5px] mb-[30px] uppercase">login to continue</p>
            <p class="font-[500] text-[14px] text-[#000000] leading-[21px] mb-[10px]">Email Address</p>
            <input class="w-[400px] mb-[25px] rounded-[6px] pl-[10px] border border-[#CCCCCC] h-[43px]" type="text" name="input" id="input" placeholder="Example@gmail.com">
            <p class="font-[500] text-[14px] text-[#000000] leading-[21px] mb-[10px]">Password</p>
            <input class="w-[400px] rounded-[6px] pl-[10px] border border-[#CCCCCC] h-[43px]" type="password" name="input" id="input" placeholder="....">
            <img class="absolute mt-[-26px] translate-x-[370px] cursor-pointer" src="../../assets/images/InputEye.svg" alt="InputEye">
            <p class="font-[400] text-[#999999] text-[14px] mt-[9px]">Forget Password ?</p>
            <div class="w-[113px] h-[1px] bg-[#999999] mb-[40px]"></div>
            <button class="py-[15px] rounded-[10px] mb-[15px] text-[#FFFFFF] px-[48px] bg-[#1ABA1A]">LOGIN</button>
            <p class="uppercase text-[#666666] text-[14px]">new user ? <span class="text-[#1ABA1A]">Sign Up</span></p>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>
<script setup lang="ts">
</script>