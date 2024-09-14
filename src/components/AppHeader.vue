<template>
  <header class="header-container">
    <div class="header-content">
      <img src="../../img/favicon.ico" alt="logo" class="logo">
      <nav class="navbar">
        <ul>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Collectibles</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">Fans</a></li>
          <li><a href="#">News</a></li>
          <li><a href="#">Shop</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
  
</script>

<style lang="scss" scoped>
$header-bg: #000;
$link-color: #fff;
$hover-color: #0074e8;

.header-container {
  padding: 1.25rem 0;
  background-color: $header-bg;
  text-align: center;

  .header-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 62.5rem;
    margin: 0 auto;
  }

  .logo {
    width: 6.25rem;
  }

  .navbar {
    ul {
      display: flex;
      gap: 1.25rem;
      padding: 0;
      margin: 0;
      list-style: none;

      li {
        a {
          color: $link-color;
          text-decoration: none;
          font-size: 1rem;
          padding: 0.5rem;
          transition: color 0.3s;

          &:hover {
            color: $hover-color;
          }
        }
      }
    }
  }
}
</style>
