<template>
    <div>
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
       
       <section id="footer-bottom">
           <div class="container-center">
               <!-- sing-up -->
               <div id="sign-up">
                   <h3>SIGN-UP NOW!</h3>
               </div>

               <!-- social channels  -->
               <div id="social-channels">
                   <span>FOLLOW US</span>
                   <ul id="social-icons">
                       <li v-for="channel, i in socialMediaChannels" :key="i">
                           <a :href="channel.url">
                               <img :src="require(`../assets/img/${channel.image}`)" :alt="channel.alt">
                           </a>
                       </li>
                   </ul>
               </div>
           </div>
       </section>
    </div>
    
</template>

<script>
export default {
  name: 'Footer',
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

          socialMediaChannels: [
              {
                  url: '#',
                  image: 'footer-facebook.png',
                  alt: 'facebook logo'
              },
              {
                  url: '#',
                  image: 'footer-twitter.png',
                  alt: 'twitter logo'
              },
              {
                  url: '#',
                  image: 'footer-youtube.png',
                  alt: 'youtube logo'
              },
              {
                  url: '#',
                  image: 'footer-pinterest.png',
                  alt: 'pinterest logo'
              },
              {
                  url: '#',
                  image: 'footer-periscope.png',
                  alt: 'periscope logo'
              }
          ]
      }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .container-center {
        width: 75%;
        margin: 0 auto;
        display: flex;
    }

    #footer-up {
        height: 130px;
        background-color: rgba(2,130,249,255);
        display: flex;

        .container-center {
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

    #footer-center {
        height: 400px;
        background-image: url("../assets/img/footer-bg.jpg");

        .container-center {
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

    #footer-bottom {
        height: 100px;
        background-color: rgba(48,48,48,255);
        display: flex;

        .container-center {
            justify-content: space-between;
            align-items: center;

            #sign-up {
                border: 2px solid rgba(5,123,232,255);
                padding: 15px;
                color: white;
                cursor: pointer;
                transition: all .8s ease;

                &:hover {
                    background-color: rgba(5,123,232,255);
                }
            }

            #social-channels {
                display: flex;
                align-items: center;

                span {
                    margin-right: 15px;
                    color: rgba(8,120,222,255);
                    font-weight: bold;
                }

                ul li {
                    display: inline;
                    margin: 0 5px;

                    &:hover {
                        cursor: pointer;
                        filter: grayscale(0.80);
                    }
                }
            }
        }

    }
</style>