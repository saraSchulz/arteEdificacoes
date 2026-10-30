<template>
  <section class="contato">
  <h3>
      Entre em Contato
  </h3>
<ul>
  <li>
    <button class="btn">
      <i class="mdi mdi-whatsapp"></i>
      WhatsApp
    </button>
    +55 (47) 99199-6242
  </li>
  <li>
    <button class="btn">
      <i class="mdi mdi-email"></i>
      Email
    </button>
    arteseedificacoes@gmail.com
  </li>
</ul>
  </section>
</template>
<style scoped>
.contato{
  background: linear-gradient(110deg, #CAA3E6 0%,#9E00FE 30% ,#CAA3E6 100%);
  min-height: 70vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  margin: 80px 0;
  color: #fff;
  box-shadow: 0 0 75px rgba(0, 0, 0, 0.8);

  & h3{
    text-align: center;
    width: 60%;
    font-size: 3rem;
    text-align: center;
    margin-top: 0.5rem;
  }
  ul{
    list-style-type: none;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    margin-top: 5rem;
    & li{
      display: flex;
      align-items: center;
      gap: 1rem;
      font-size: 2rem;

      & .btn{
        background-color: #CAA3E6;
        border: none;
        padding: 0.5rem 5rem;
        border-radius: 50px;
        cursor: pointer;
        transition: all 0.5s ease-in-out;
        display: flex;
        justify-content: center;
        align-items: center;
        box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.5);

        & i{
          margin-right: 1rem;
          font-size: 2rem;
          color: #000;
        }
      }
    }
  }
}
</style>
