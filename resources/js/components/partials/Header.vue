<template>
  <header>
    <div class="container">
      <nav>
        <ul>
          <li><a href="">Home</a></li>
          <li><a href="">Blog</a></li>
          <li><a href="">Contatti</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="scss" scoped>
  header {
    height: 70px;

    background-color: cornflowerblue;
    nav {
      height: 100%;
      line-height: 70px;
      ul {
        list-style: none;
        li {
          display: inline-block;
          margin-right: 10px;
          a {
            text-decoration: none;
            color: black;
            &:hover {
              color: white;
            }
          }
        }
      }
    }
  }
</style>