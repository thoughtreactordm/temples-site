<template>
  <div class="layout">
    <!--<header class="header">
      <strong>
        <g-link to="/">{{ $static.metaData.siteName }}</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/">Home</g-link>
        <g-link class="nav__link" to="/about">About</g-link>
      </nav>
    </header>-->
    <slot/>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<style>
  @import url('https://fonts.googleapis.com/css?family=Lato:300,400,700,900&display=swap');

  html, body {
    height: 100vh;
  }

  body {
    margin: 0;
    padding: 0;

    height: 100%;

    background-color: #4d3a5e;
    background: url("../assets/img/splash.png");
    background-size: cover;
    background-position: center;

    font-family: 'Lato', sans-serif;

    color: white;
    text-shadow: 1px 2px 2px rgba(0,0,0,0.5);
  }
</style>
