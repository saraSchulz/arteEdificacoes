<template>
  <section class="sobre">
  <h3>
    Há decadas  fazendo da excelência o nosso compromisso.
  </h3>
  <button class="btn">
    <a href="https://www.facebook.com/profile.php?id=61591919670765&locale=pt_BR" target="_blank">
      <i class="mdi mdi-facebook"></i>
    Acesse nosso facebook
    </a>
  </button>
</section>
</template>
<style scoped>
.sobre{
  min-height: 40vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  margin: 20px 0;
  & h3{
    text-align: center;
    width: 60%;
    font-size: 3rem;
    text-align: center;
    margin-top: 5rem;
    color: #9E00FE;
  }
  .btn{
    margin-top: 5rem;
    background-color: #9E00FE;
    border: none;
    padding: 1rem 2rem;
    border-radius: 50px;
    cursor: pointer;
    transition: all 0.5s ease-in-out;
    width: 40%;
    align-items: center;
    color: #fff;
    display: flex;
    justify-content: center;

    & a{
      text-decoration: none;
      color: #fff;
      font-size: 1.5rem;
      gap: 1rem;
    }
    &:hover{
      background-color: #7A00C2;
    }
    & i{
      font-size: 2rem;
      color: #fff;
    }
  }
}
</style>
