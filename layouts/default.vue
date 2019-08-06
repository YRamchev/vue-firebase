<template>
  <div class="page-wrapper">
    <header class="header">
      <div class="header__logo">
        <nuxt-link :to="{name: 'index'}">
          <img src="/logo.png" alt="">
        </nuxt-link>
      </div>
      <nav class="nav-wrapper">
        <ul class="nav">
          <li class="nav__item">
            <nuxt-link :to="{name: 'index'}" class="nav__link">
              My Work
            </nuxt-link>
          </li>
          <li class="nav__item">
            <nuxt-link :to="{name: 'shop'}"  class="nav__link">
              Shop
            </nuxt-link>
          </li>
          <li class="nav__item">
            <nuxt-link :to="{name: 'about'}" class="nav__link">
              About Me
            </nuxt-link>
          </li>
          <li class="nav__item">
            <nuxt-link :to="{name: 'contacts'}" class="nav__link">
              Contact Me
            </nuxt-link>
          </li>
        </ul>
      </nav>
    </header>

    <main class="content-wrapper">
      <nuxt />
    </main>  
      
    <footer class="footer">

    </footer>
  </div>
</template>

<style scoped>
  html {
    font-size: 100%;
  }

  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
  }

  .header__logo img {
    max-width: 128px;
  }

  .nav {
    display: flex;
    list-style-type: none;
  }

  .nav__link {
    display: block;
    font-size: 1.3rem;
    text-decoration: none;
    text-transform: uppercase;
    padding: 1rem;
    position: relative;
    color: rgba(0, 0, 0, .57)
  }

  .nav__link.nuxt-link-active,
  .nav__link:hover {
    color: rgba(0, 0, 0, .87)
  }

  .content-wrapper {
    margin: 0 auto;
    max-width: 1600px;
    padding: 4rem 0;
  }
</style>