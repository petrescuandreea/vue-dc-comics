<template>
    <header>
      <div class="container-center">
        <!-- logo  -->
        <img src="../assets/img/dc-logo.png" alt="logo DC">

        <!-- nav menu  -->
        <nav>
          <ul>
            <li v-for="link, i in links" :key="i">
              <a :href="link.url" :class="link.here ? 'active' : ''">{{ link.text }}</a>
            </li>
          </ul>
        </nav>
      </div>
    </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      links: [
        {
          text:"CHARACTERS",
          url:"#",
          here: false,
        },
        {
          text:"COMICS",
          url:"#",
          here: true,
        },
        {
          text:"MOVIES",
          url:"#",
          here: false,
        },
        {
          text:"TV",
          url:"#",
          here: false,
        },
        {
          text:"GAMES",
          url:"#",
          here: false,
        },
        {
          text:"COLLECTIBLES",
          url:"#",
          here: false,
        },
        {
          text:"VIDEOS",
          url:"#",
          here: false,
        },
        {
          text:"FANS",
          url:"#",
          here: false,
        },
        {
          text:"NEWS",
          url:"#",
          here: false,
        },
        {
          text:"SHOP",
          url:"#",
          here: false,
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  header {
    height: 120px;
    display: flex;

    img {
      max-width: 80px;
    }

    div {
      width: 75%;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;

      li {
        display: inline-block;
        margin: 0 10px;

        a {
          text-decoration: none;
          color: rgba(142,140,142,255);
          font-size: 10px;
          font-weight: bold;
          padding: 48px 5px;
        }
      }
    }

  }

</style>