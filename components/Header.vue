<template>
  <header class="header">
    <div class="header-inner">
      <div class="logo"></div>
      <nav class="menu_m">
        <ul class="menu">
          <li class="menu-item">
            <span class="menu-item-label">Explore</span>
            <svg
              class="menu-item-arrow"
              width="8"
              height="5"
              viewBox="0 0 8 5"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M1.5 1.5L4 4L7 1.5"
                stroke="black"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </li>
          <li class="menu-item">
            <span class="menu-item-label">Company</span>
            <svg
              class="menu-item-arrow"
              width="8"
              height="5"
              viewBox="0 0 8 5"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M1.5 1.5L4 4L7 1.5"
                stroke="black"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </li>
          <li class="menu-item">
            <span class="menu-item-label">Pricing</span>
          </li>
          <li class="menu-item">
            <span class="menu-item-label">Blog</span>
          </li>
        </ul>
      </nav>
      <nav class="umenu">
        <ul class="umenua">
          <li>Experience Our Tech</li>
          <li class="button">
            <span class="button-b"></span>
            <span class="button-h"></span>
            <span class="button-t">Demo</span>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
.header {
  width: 100%;
  top: 0;
  left: 0;
  font-size: 0.875rem;
  font-weight: 600;
  z-index: 100;
}

.header-inner {
  display: flex;
  flex-direction: row;
  top: 20px;
  width: 80%;
  height: 60px;
  margin: auto;
  justify-content: space-between;
  position: relative;
  align-items: center;
}

.logo {
  background: black;
  width: 3.75rem;
  height: 3.75rem;
  margin-right: 1.875rem;
}

.menu {
  list-style: none;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
}

.umenu {
  width: 50%;
}

.umenua {
  list-style: none;
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
}

.menu-item {
  margin-right: 2rem;
  position: relative;
}

.menu-item-label {
  display: block;
  text-decoration: none;
  z-index: 2;
}
.menu-item-arrow {
  position: absolute;
  top: 0.35rem;
  right: -0.85rem;
  z-index: 2;
}

nav {
  display: block;
}

.button-h{
  border-radius: 50%;
  bottom: 0;
  left: 50%;
  transform: translate(-50%,50%) scale(0);
  transition: transform .5s cubic-bezier(0.165, 0.84, 0.44, 1);
  will-change: transform;
  background-color: #1e2432;
}

.button:hover .button-h{
  transform: translate(-50%, 50%) scale(1);
}

.button-b{
  top:0;
  left: 0;
  width: 100%;
  height:100%;
  opacity: 1;
  transition: opacity 0.5s cubic-bezier(0.165, 0.84, 0.44, 1);
}

.button-b:hover{
  opacity: 0;
}

.button{
  padding: 0.68rem 1.25rem .75rem;
}
</style>