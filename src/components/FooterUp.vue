<template>
    <section id="footer-up">
        <div class="container-center">
                <nav>
                    <ul>
                        <li v-for="item, i in footerNav" :key="i">
                            <a :href="item.url">
                                <img :src="require(`../assets/img/${item.image}`)" :alt="item.text">{{ item.text }}
                            </a>
                        </li>
                    </ul>
                </nav>
        </div>
    </section>
</template>

<script>
export default {
  name: 'FooterUp',
  data() {
      return {
          footerNav: [
              {
                  url: '#',
                  image:'buy-comics-digital-comics.png',
                  text:'DIGITAL COMICS'
              },
              {
                  url: '#',
                  image:'buy-comics-merchandise.png',
                  text:'DC MERCHANDISE'
              },
              {
                  url: '#',
                  image:'buy-comics-subscriptions.png',
                  text:'SUBSCRIPTION'
              },
              {
                  url: '#',
                  image:'buy-comics-shop-locator.png',
                  text:'COMIC SHOP LOCATOR'
              },
              {
                  url: '#',
                  image:'buy-dc-power-visa.svg',
                  text:'DC POWER VISA'
              }
            ],
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #footer-up {
        padding: 55px 0;
        background-color: rgba(2,130,249,255);

        .container-center {
        width: 75%;
        margin: 0 auto;

            ul{
                display: flex;
                justify-content: space-evenly;

                li{
                    display: inline-block;
                    margin-right: 25px;

                    a {
                        font-size: 14px;
                        color: white;
                        text-decoration: none;
                        display: flex;
                        align-items: center;

                        img {
                            
                            height: 50px;
                            margin-right: 10px;
                        }
                    }


                }
            }
        }
    }

</style>