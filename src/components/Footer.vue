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
                       <h3>DC COMICS</h3>
                       <nav>
                           <ul>
                               <li>
                                   <a href="#">Characters</a>
                               </li>
                               <li>
                                   <a href="#">Comics</a>
                               </li>
                               <li>
                                   <a href="#">Movies</a>
                               </li>
                               <li>
                                   <a href="#">TV</a>
                               </li>
                               <li>
                                   <a href="#">Games</a>
                               </li>
                               <li>
                                   <a href="#">Videos</a>
                               </li>
                               <li>
                                   <a href="#">News</a>
                               </li>
                               <li id="second-nav">
                                   <a href="#">SHOP</a>
                               </li>
                               <li>
                                   <a href="#">Shop DC</a>
                               </li>
                               <li>
                                   <a href="#">Shop DC Collectubles</a>
                               </li>
                           </ul>
                       </nav>

                   </div>

                   <div id="dc-nav">
                       <h3>DC</h3>
                       <nav>
                           <ul>
                               <li>
                                   <a href="#">Terms Of Use</a>
                               </li>
                               <li>
                                   <a href="#">Privacy policy (New)</a>
                               </li>
                               <li>
                                   <a href="#">Ad Choices</a>
                               </li>
                               <li>
                                   <a href="#">Advertising</a>
                               </li>
                               <li>
                                   <a href="#">Jobs</a>
                               </li>
                               <li>
                                   <a href="#">Subscriptions</a>
                               </li>
                               <li>
                                   <a href="#">Talent Workshops</a>
                               </li>
                               <li>
                                   <a href="#">CPSC Certificates</a>
                               </li>
                               <li>
                                   <a href="#">Ratings</a>
                               </li>
                               <li>
                                   <a href="#">Shop Help</a>
                               </li>
                               <li>
                                   <a href="#">Contact Us</a>
                               </li>
                           </ul>
                       </nav>
                   </div>

                   <div id="sites-nav">
                       <h3>SITES</h3>
                       <nav>
                           <ul>
                               <li>
                                   <a href="#">DC</a>
                               </li>
                               <li>
                                   <a href="#">MAD Magazine</a>
                               </li>
                               <li>
                                   <a href="#">DC Kids</a>
                               </li>
                               <li>
                                   <a href="#">DC Universe</a>
                               </li>
                               <li>
                                   <a href="#">DC Power Visa</a>
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
                       <li>
                           <img src="../assets/img/footer-facebook.png" alt="facebook logo">
                       </li>
                        <li>
                           <img src="../assets/img/footer-twitter.png" alt="twitter logo">
                       </li>
                        <li>
                           <img src="../assets/img/footer-youtube.png" alt="youtube logo">
                       </li>
                        <li>
                           <img src="../assets/img/footer-pinterest.png" alt="pinterest logo">
                       </li>
                        <li>
                           <img src="../assets/img/footer-periscope.png" alt="persicope logo">
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
          ]
      }
  }
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
                    
                    h3, #second-nav {
                            color: white;
                            font-size: 15px;
                            margin: 20px 0 15px 0;
                        }

                        #second-nav a {
                            color: white;
                            font-size: 15px;
                            font-weight: bold;
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