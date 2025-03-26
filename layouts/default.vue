<template>
    <div class="fullwidth">
      <nav>
        <ul>
          <li><NuxtLink to="/" class="nav-btn" exact-active-class="active">Home</NuxtLink></li>
          <li><NuxtLink to="/about" class="nav-btn" exact-active-class="active">About</NuxtLink></li>
          <li><NuxtLink to="/contact" class="nav-btn" exact-active-class="active">Contact</NuxtLink></li>
          <li><NuxtLink to="/projects" class="nav-btn" exact-active-class="active">Projects</NuxtLink></li>
        </ul>
      </nav>
  
      <main>
        <Nuxt />
      </main>
    </div>
  </template>
  
  <style scoped>
  /* Navigation container */
  nav {
    display: flex;
    justify-content: center;
    padding: 20px;
  }
  
  /* Navigation list */
  nav ul {
    list-style: none;
    display: flex;
    gap: 15px;
    padding: 0;
    margin: 0;
  }
  
  /* Styled Navigation Buttons */
  .nav-btn {
    display: inline-block;
    width: 160px;
    height: 50px;
    border-radius: 12px;
    border: none;
    font-family: "Raleway-VariableFont_wght", sans-serif;
    font-size: 20px;
    color: rgb(68, 149, 68);
    text-align: center;
    line-height: 50px;
    text-decoration: none;
    cursor: pointer;
    transition: background 0.3s ease-in-out;
  }
  
  /* Hover effect */
  .nav-btn:hover {
    background: rgba(227, 243, 221, 0.826);
  }
  
  /* Keep hover color on the active page */
  .active {
    background: rgba(227, 243, 221, 0.312);
  }
  </style>
  