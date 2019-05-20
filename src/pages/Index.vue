<template>
  <Layout>
    
    <div class="content">
      <!-- Learn how to use images here: https://gridsome.org/docs/images -->
      <g-image alt="Example image" src="~/assets/img/logo.png" class="logo" />

      <h1>Official Site Coming Soon!</h1>

      <div>
        <a href="https://instagram.com/templesofigeo" class="social">
          <font-awesome-icon :icon="['fab', 'instagram']"/>
        </a>
        <a href="https://twitter.com/templesofigeo" class="social">
          <font-awesome-icon :icon="['fab', 'twitter']"/>
        </a>
        <a href="https://youtube.com/TheThoughtReactor" class="social">
          <font-awesome-icon :icon="['fab', 'youtube']"/>
        </a>
      </div>
    </div>



  </Layout>
</template>

<script lang="scss">
export default {
  metaInfo: {
    title: 'Site Coming Soon'
  }
}
</script>

<style lang="scss">
  .logo {
    width: 100%;
    max-width: 750px;
  }

  div.content {
    background-color: rgba(0,0,0,0.5);
    width: 100vw;
    height: 100vh;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    a.social {
      font-size: 2rem;
      color: #FFC135;
      margin: 16px;

      transition: all 0.1s ease-in-out;

      &:hover {
        color: darken(#FFC135, 15%);
        filter: drop-shadow(0 1px 6px rgba(255, 193, 53, 0.3));
      }
    }
  }
</style>
