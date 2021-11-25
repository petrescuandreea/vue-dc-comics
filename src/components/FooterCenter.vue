<template>
    <section id="footer-center">
           <div class="container-center">
               <div id="footer-nav">
                   <div id="dc-comics-shop-nav">
                       <nav>
                           <ul>
                               <h3>DC COMICS</h3>
                               <li v-for="link, i in dcComicsLinks" :key="i">
                                   <a :href="link.url">{{ link.text }}</a>
                               </li>
                           </ul>
                       </nav>

                       <nav>
                           <ul>
                               <h3>SHOP</h3>
                               <li v-for="link, i in shopLinks" :key="i">
                                   <a :href="link.url">{{ link.text }}</a>
                               </li>
                           </ul>
                       </nav>
                   </div>

                   <div id="dc-nav">
                       <nav>
                           <ul>
                               <h3>DC</h3>
                               <li v-for="link, i in dcLinks" :key="i">
                                   <a :href="link.url">{{ link.text }}</a>
                               </li>
                           </ul>
                       </nav>
                   </div>

                   <div id="sites-nav">
                       <nav>
                           <ul>
                               <h3>SITES</h3>
                               <li v-for="link, i in sitesLinks" :key="i">
                                   <a :href="link.url">{{ link.text }}</a>
                               </li>
                           </ul>
                       </nav>
                   </div>
               </div>

               <div id="logo">
                   <img src="../assets/img/dc-logo-bg.png" alt="dc logo">
               </div>
           </div>
       </section>
</template>

<script>
export default {
  name: 'FooterCenter',
  data() {
      return {
          dcComicsLinks: [
              {
                  url:'#',
                  text:'Characters'
              },
              {
                  url:'#',
                  text:'Comics'
              },
              {
                  url:'#',
                  text:'Movies'
              },
              {
                  url:'#',
                  text:'TV'
              },
              {
                  url:'#',
                  text:'Games'
              },
              {
                  url:'#',
                  text:'Videos'
              },
              {
                  url:'#',
                  text:'News'
              }
          ],

          shopLinks: [
              {
                  url: '#',
                  text:'Shop DC'
              },
              {
                  url: '#',
                  text: 'Shop DC Collectibles'
              }
          ],

          dcLinks: [
              {
                  url:'#',
                  text:'Terms Of Use'
              },
              {
                  url:'#',
                  text:'Privacy policy (New)'
              },
              {
                  url:'#',
                  text:'Ad Choices'
              },
              {
                  url:'#',
                  text:'Advertising'
              },
              {
                  url:'#',
                  text:'Jobs'
              },
              {
                  url:'#',
                  text:'Subscriptions'
              },
              {
                  url:'#',
                  text:'Talent Workshops'
              },
              {
                  url:'#',
                  text:'CPSC Certificates'
              },
              {
                  url:'#',
                  text:'Ratings'
              },
              {
                  url:'#',
                  text:'Shop Help'
              },
              {
                  url:'#',
                  text:'Contact Us'
              },
          ],

           sitesLinks: [
              {
                  url:'#',
                  text:'DC'
              },
              {
                  url:'#',
                  text:'MAD Magazine'
              },
              {
                  url:'#',
                  text:'DC Kids'
              },
              {
                  url:'#',
                  text:'DC Universe'
              },
              {
                  url:'#',
                  text:'DC Power Visa'
              }
          ],
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #footer-center {
        height: 400px;
        background-image: url("../assets/img/footer-bg.jpg");

        .container-center {
            width: 75%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;

            #footer-nav {
                float: left;
                display: flex;
                margin: 50px 0;

                #dc-comics-shop-nav,
                #dc-nav,
                #sites-nav {
                    margin-right: 30px;
                    
                    h3 {
                        color: white;
                        font-size: 15px;
                        margin: 20px 0 15px 0;
                    }

                    li {
                        list-style-type: none;

                        a {
                            color: #5c5c5c;
                            font-size: 10px;
                            text-decoration: none;

                            &:hover {
                                color: #0282F9;
                            }
                        }
                    }

                }
            }

            #logo {
                float: right;

                img {
                        width: 600px;
                        height: 400px;
                        object-fit: none;
                }
            }
        }
    }

</style>