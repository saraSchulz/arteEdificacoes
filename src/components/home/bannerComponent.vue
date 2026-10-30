<template>
<section class="banner">
  <h1>
    Schulz
  </h1>
  <h2>
    Arte e Edificações
  </h2>
</section>

</template>
<style scoped>
.banner{
   background: url(/banner-img.png) no-repeat center center/cover;
   min-height: 100vh;
   display: flex;
   flex-direction: column;
   justify-content: center;
    text-align: center;
    box-shadow: 0 0 50px rgba(0, 0, 0, 0.75);
    & h1{
      font-size: 9rem;
      color: #fff;
    }
    & h2{
      font-size: 5rem;
      color: #fff;
      margin-top: -2rem;
    }
}
</style>
