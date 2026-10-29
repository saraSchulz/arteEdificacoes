<script setup></script>

<template>
  <footer>
    <div class="left">
      <h3>Redes Sociais e contato</h3>
      <ul>
        <li>
          <a href="https://www.facebook.com/profile.php?id=61591919670765&locale=pt_BR">
          <i class="mdi mdi-facebook"></i>
          A Schulz- arte e edificações
          </a>
        </li>
        <li>
          <a href="https://wa.me/5547991996242">
          <i class="mdi mdi-whatsapp"></i>
          +55 (47) 99199-6242
          </a>
        </li>
        <li>
          <a href="https://www.facebook.com/profile.php?id=61591919670765&locale=pt_BR">
          <i class="mdi mdi-email"></i>
          arteedificacaoschulz@gmail.com
          </a>
        </li>
      </ul>
      </div>
      <div class="right">
        <div class="logoFooter">
          <RouterLink to="/">
          <img src="/logo.png" alt="logo" class="logo" />
        </RouterLink>
        </div>
        <div class="direitos">
          <p>Desenvolvido por Sara Schulz</p>
          <p>&copy; Alguns direitos reservados</p>

        </div>
      </div>


  </footer>
</template>

<style scoped>
footer {
    background:
    radial-gradient(ellipse at 55% 50%,rgba(190, 40, 255, 0.9) 0%, transparent 65%),
    linear-gradient(110deg,#6500A8 0%,#9E00FE 55%,#8500D8 100%);
    display: flex;
    justify-content: space-between;
    whidth: 100%;
    padding: 20px;
    color: white;

    & .left{
      width: 40%;
      font-size: 1rem;
      margin-left: 20px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      text-align: center;
      & h3{
        font-size: 1.5rem;
      }
      & ul{
        list-style: none;
        & li{
          margin: 10px 0;
          & a{
            color: white;
            text-decoration: none;
            & i{
              margin-right: 10px;
              font-size: 1.5rem;
            }
          }
        }
      }
    }
    & .right{
      width: 40%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      & .logoFooter{
        display: flex;
        align-items: center;
        justify-content: center;
        & img{
          width: 40%;
          height: auto;
          margin-right: 10px;
        }
        & a{
          color: white;
          text-decoration: none;
          font-size: 1.5rem;
        }
      }
      & .direitos{
        text-align: center;
        & p{
          margin: 5px 0;
        }
      }
    }
}
</style>
