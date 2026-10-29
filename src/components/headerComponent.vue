<script setup>
</script>

<template>
  <header>
    <!-- Menu hamburguer (agora fica à esquerda) -->
    <div class="menu-hamburguer">
      <input type="checkbox" id="menu-toggle" />
      <label for="menu-toggle" class="menu-icon">
        <div class="linha"></div>
        <div class="linha"></div>
        <div class="linha"></div>
      </label>

      <!-- Overlay escuro (fora do menu) -->
      <label for="menu-toggle" class="backdrop"></label>

      <!-- Menu lateral -->
      <nav class="overlay">
  <div class="sidebar-content">
    <p>
      <RouterLink to="/">
        <i class="mdi mdi-home-roof"></i>
        Home
      </RouterLink>
    </p>
  </div>

  <div class="sidebar-footer">
    <RouterLink to="/">
      <img src="/logo.png" alt="Schulz Construções" class="sidebar-logo" />
    </RouterLink>
  </div>
</nav>
    </div>

    <h1 class="logo">
      <RouterLink to="/">
        <img src="/logo.png" alt="logo">
      </RouterLink>
    </h1>
  </header>
</template>

<style scoped>
/*====================================
				HEADER
=====================================*/
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;

  display: flex;
  justify-content: space-between;
  align-items: center;

  background: rgba(158, 0, 254, 0.8);
  padding: 10px 20px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.8);
}

header h1 img {
  height: 80px;
  margin: 0 20px;
}

/*============ Menu hamburguer ===========*/
.menu-hamburguer {
  z-index: 1100;
}

#menu-toggle {
  display: none;
}

.menu-icon {
  width: 35px;
  height: 30px;
  cursor: pointer;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  z-index: 1200;
  position: relative;
  transition: all 0.5s ease;
  margin: 0 20px;
}

.menu-icon:hover .linha {
  background: #000000;
}

div.linha {
  height: 4px;
  background: #ffffff;
  border-radius: 2px;
  box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.5);
  transition: all 1s ease;
}

/*============ Overlay escuro fora do menu ===========*/
.backdrop {
  position: fixed;
  inset: 0;
  background: rgba(0, 0, 0, 0.7);
  opacity: 0;
  pointer-events: none;
  transition: opacity 0.4s ease;
  z-index: 900;
}

#menu-toggle:checked~.backdrop {
  opacity: 1;
  pointer-events: auto;
}


.overlay {
  position: fixed;
  top: 0;
  left: 0;

  width: 30%;
  max-width: 350px;
  height: 100vh;
  box-sizing: border-box;

  background: #9E00FE;
  transform: translateX(-100%);
  transition: transform 0.4s ease-in-out;

  z-index: 1000;
  padding: 40px 20px;
  box-shadow: 5px 0 15px rgba(0, 0, 0, 0.5);

  /* Organiza o conteúdo verticalmente */
  display: flex;
  flex-direction: column;
}

#menu-toggle:checked ~ .overlay {
  transform: translateX(0);
}


/* Conteúdo superior */
.sidebar-content {
  flex: 1;
}

.overlay p {
  font-size: 40px;
  margin: 40px 0;
}

.overlay p a {
  text-decoration: none;
  color: #ffffff;
  transition: color 0.3s ease;

  display: flex;
  align-items: center;
  gap: 10px;

  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.75);
}

.overlay p a:hover {
  color: #000000;
}

/* Logo fixada na parte inferior */
.sidebar-footer {
  margin-top: auto;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
}

.sidebar-footer a {
  display: block;
  width: 100%;
  text-align: center;
}

.sidebar-logo {
  display: block;
  width: 100%;
  max-width: 180px;
  height: auto;
  margin: 0 auto;
}

#menu-toggle:checked~.overlay {
  transform: translateX(0);
}

/*============ Menu interno ===========
mudanças futuras no menu interno
.menu-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.menu-list li {
  margin: 20px 0;
}
*/
.overlay p{
  font-size: 40px;
  margin: 40px 0;
}
.overlay p a {
  text-decoration: none;
  color: #ffffff;
  transition: color 1s ease;
  display: flex;
  align-items: center;
  gap: 10px;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.75);
}
.overlay p a:hover {
  color: #000000;
}

.overlay .logo {
   width: 100%;
  max-width: 180px;
  height: auto;
  bottom: 10px;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.75);
}
</style>
