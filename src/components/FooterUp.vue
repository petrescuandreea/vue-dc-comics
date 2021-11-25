<template>
    <section id="footer-up">
        <div class="container-center">
            <div v-for="item, i in footerNav" :key="i" class="card">
                <div class="card-content">
                    <img :src="require(`../assets/img/${item.image}`)" :alt="item.text">
                    <span>{{ item.text }}</span>
                </div>
                
            </div>
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
                  image:'buy-comics-digital-comics.png',
                  text:'DIGITAL COMICS'
              },
              {
                  image:'buy-comics-merchandise.png',
                  text:'DC MERCHANDISE'
              },
              {
                  image:'buy-comics-subscriptions.png',
                  text:'SUBSCRIPTION'
              },
              {
                  image:'buy-comics-shop-locator.png',
                  text:'COMIC SHOP LOCATOR'
              },
              {
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
        height: 130px;
        background-color: rgba(2,130,249,255);
        display: flex;

        .container-center {
        width: 75%;
        margin: 0 auto;
        display: flex;
        justify-content: space-evenly;

            .card {
                display: flex;
                align-items: center;

                .card-content {
                    display: flex;
                    align-items: center;
                    cursor: pointer;

                    img {
                    max-width: 35px;
                    max-height: 35px;
                    margin-right: 5px;
                    }

                    span {
                        font-size: 12px;
                        color: white;
                    }
                }
            }
        }
    }

</style>