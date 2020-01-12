<template>

  <header>
    <nav>
      <div class='container'>
        <ul>
          <li>
            <div class="side-menu-container">
                  
            </div>
          </li>
          <li>
            <div class="imagen-perfil">
              <img src="../assets/perfil-resilencia.jpg" alt="">
            </div>
          </li>
          <li>
            <div class="imagen-perfil">
              <img src="../assets/perfil-resilencia.jpg" alt="">
            </div>
          </li>

        </ul>
      </div>
    </nav>
  </header>
</template>

<style lang="css">
  @import url(https://fonts.googleapis.com/css?family=Montserrat:400,700);

  @import url(http://weloveiconfonts.com/api/?family=fontawesome);

  [class*="fontawesome-"]:before {
    font-family: 'FontAwesome', sans-serif;
  }

  * {
    box-sizing: border-box;
  }

  *:before,
  *:after {
    box-sizing: border-box;
  }



  nav {
    width: 100%;
  }

  nav ul {
    padding: 0;
    margin: 0;
    list-style-type: none;
    float: center;
    text-align: center;
  }

  nav li {
    display: inline-block;
    padding: 2em;
    text-align: center;
    transition: all .2s;
  }

  nav li:last-child {
    padding-right: 0;
  }

  header {
    position: relative;
  }

  .imagen-perfil {
    border-radius: 50px;
    width: 75px;
    height: 75px;
    overflow: hidden;
  }

  .imagen-perfil img {
    overflow: hidden;
    width: 180px;
    height: 75px;
  }
</style>