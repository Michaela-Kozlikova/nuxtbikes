<template>
  <div class="page-wrapper">
    <header>
      <div class="header-bar">
        <div class="website-logo">
          <NuxtLink to="/">
            <img
              src="/pics/website-logo.png"
              alt="Logo"
              width="100"
              height="90"
            />
          </NuxtLink>
        </div>
      <h1>Svět japonských motorek: výkon na dosah</h1>
      <p>Precizní technika na dvou kolech</p>
    </div>
      <nav id="main-nav">
        <NuxtLink to="/honda">Honda</NuxtLink>
        <NuxtLink to="/suzuki">Suzuki</NuxtLink>
        <NuxtLink to="/kawasaki">Kawasaki</NuxtLink>
        <NuxtLink to="/yamaha">Yamaha</NuxtLink>
      </nav>
    </header>

    <slot />

    <footer class="site-footer">
      <div class="footer-icons">
        <img src="/pics/icons/youtube.png" />
        <img src="/pics/icons/facebook.png" />
        <img src="/pics/icons/instagram.png" />
      </div>
      <p class="footer-credit">Made with ❤ by Misha</p>
    </footer>
  </div>
</template>

<style>
* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #2b2a2a;
  color: white;
}

.page-wrapper {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
}

header {
  display: flex;
  width: 100%;
  align-items: center;
  flex-direction: column;
  padding-top: 10px;
  margin-top: 0;
}

.header-bar {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  width: 100%;
  flex-direction: column;
}

.website-logo {
   position: absolute; 
   left: 10px;
   top: 20px;
}

.website-logo img {
  border-radius: 10px;
}

#main-nav {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 80px;
  margin-top: 40px;
  padding: 2px 0;
  border-top: 3px solid white;
  border-bottom: 3px solid white;
  width: 100%;
}

#main-nav a {
  text-decoration: none;
  color: rgba(208, 150, 205, 0.785);
  font-weight: bold;
}

#main-nav a:hover {
  transform: scale(1.2);
  transition: 0.3s;
  text-shadow: 0 0 rgb(21, 20, 20);
  border-radius: 30%;
  margin: 2;
}

.site-footer {
  margin-top: auto;
}

.footer-credit {
  display: flex;
  align-items: center;
  justify-content: center;
  padding-top: 14px;
}

.footer-icons {
  display: flex;
  gap: 20px;
  justify-content: center;
}

.footer-icons img {
  width: 34px;
}

footer .footer-icons img:hover {
  transform: scale(1.3);
  transition: 0.4s;
  cursor: pointer;
}
</style>
