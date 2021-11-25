<template>
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
</template>

<script>
export default {
  name: 'FooterBottom',
  data() {
      return {
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
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    #footer-bottom {
        height: 100px;
        background-color: rgba(48,48,48,255);
        display: flex;

        .container-center {
            width: 75%;
            margin: 0 auto;
            display: flex;
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