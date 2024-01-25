<template>
  <v-app dark>



    <v-app-bar fixed app class="elevation-0" height="auto" style="padding-top: 15px; padding-bottom: 15px;">


      <v-toolbar-title style="font-family: 'Titan One', sans-serif; color: #612009;"> DONUT DISTURB</v-toolbar-title>

      <v-img :src="require('@/assets/donut-icon.png')" alt="Logo" contain max-height="40" max-width="40"
        style="margin-left: 10px;"></v-img>

      <v-spacer />


      <router-link to="/">
        <v-btn text class="hidden-sm-and-down" style="font-family: Arial, Helvetica, sans-serif; color: #612009;">
          HOME
        </v-btn>
      </router-link>

      <v-btn text class="hidden-sm-and-down" style="font-family: Arial, Helvetica, sans-serif; color: #612009;"
        @click="scrollToSection('#our-story')">
        OUR STORY
      </v-btn>

      <v-btn text class="hidden-sm-and-down" style="font-family: Arial, Helvetica, sans-serif; color: #612009;"
        @click="scrollToSection('#reviews')">
        REVIEWS
      </v-btn>

      <v-btn text class="hidden-sm-and-down" style="font-family: Arial, Helvetica, sans-serif; color: #612009;"
        @click="scrollToSection('#contact-us')">
        CONTACT US
      </v-btn>

      <v-btn icon class="hidden-sm-and-down">
        <v-icon size="24" color="#612009">mdi-facebook</v-icon>
      </v-btn>

      <v-btn icon class="hidden-sm-and-down">
        <v-icon size="24" color="#612009">mdi-twitter</v-icon>
      </v-btn>

      <v-btn icon class="hidden-sm-and-down">
        <v-icon size="24" color="#612009">mdi-instagram</v-icon>
      </v-btn>

      <v-btn icon class="hidden-sm-and-down">
        <v-icon size="24" color="#612009">mdi-account-circle</v-icon>
      </v-btn>


      <v-btn icon class="hidden-md-and-up" @click.stop="drawer = !drawer">
        <v-icon color="#612009">mdi-menu</v-icon>
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" app temporary class="elevation-0">
      <v-list-item-group>
        <v-list-item>
          <v-icon size="24" color="#612009">mdi-account-circle</v-icon>
        </v-list-item>
        <v-list-item>
          <v-list-item-title color="#612009">HOME</v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title color="#612009">OUR STORY</v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title color="#612009">OUR MENU</v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title color="#612009">CONTACT US</v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-icon size="24" color="#612009">mdi-facebook</v-icon>
        </v-list-item>
        <v-list-item>
          <v-icon size="24" color="#612009">mdi-twitter</v-icon>
        </v-list-item>
        <v-list-item>
          <v-icon size="24" color="#612009">mdi-instagram</v-icon>
        </v-list-item>
      </v-list-item-group>
    </v-navigation-drawer>



    <Nuxt />




    <footer class="footer-section">
      <div class="container">
        <div class="footer-cta pt-5 pb-5">
          <div class="row">
            <div class="col-xl-4 col-md-4 mb-30">
              <div class="single-cta">
                <v-icon color="white" size="40" style="margin-left: -10px;">mdi-map-marker</v-icon>
                <div class="cta-text">
                  <h4>Find us</h4>
                  <span>Dolores San Fernando Pampanga, Building 103</span>
                </div>
              </div>
            </div>
            <div class="col-xl-4 col-md-4 mb-30">
              <div class="single-cta">
                <v-icon color="white" size="40">mdi-phone</v-icon>
                <div class="cta-text">
                  <h4>Call us</h4>
                  <span>+63 9534203251</span>
                </div>
              </div>
            </div>
            <div class="col-xl-4 col-md-4 mb-30">
              <div class="single-cta">
                <v-icon color="white" size="40">mdi-email</v-icon>
                <div class="cta-text">
                  <h4>Mail us</h4>
                  <span>donutdisturb@gmail.com</span>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="footer-content pt-5 pb-5">
          <div class="row">
            <div class="col-xl-4 col-lg-4 mb-50">
              <div class="footer-widget">
                <div class="footer-logo">
                  <h1 style="font-family: 'Titan One', sans-serif; color: white">DONUT DISTURB</h1>
                </div>
                <div class="footer-text">
                  <p> Our commitment to sweetness and unwavering dedication to quality have made us the top choice for
                    discerning individuals who crave the perfect blend of flavor, texture, and satisfaction.</p>
                </div>
                <div class="footer-social-icon">
                  <span>Follow us:</span>
                  <v-icon color="white" size="30">mdi-facebook</v-icon>
                  <v-icon color="white" size="30">mdi-instagram</v-icon>
                  <v-icon color="white" size="30">mdi-twitter</v-icon>
                </div>
              </div>
            </div>
            <div class="col-xl-4 col-lg-4 col-md-6 mb-30">
              <div class="footer-widget">
                <div class="footer-widget-heading">
                  <h3>Other Links</h3>
                </div>
                <ul>
                  <li><a>Home</a></li>
                  <li><a>Our Story</a></li>
                  <li><a>Reviews</a></li>
                  <li><a>Menu</a></li>
                  <li><a>Contact us</a></li>
                  <li><a>Latest News</a></li>
                  <li><a>Opportunities</a></li>
                  <li><a>Upcoming Events</a></li>
                </ul>
              </div>
            </div>
            <div class="col-xl-4 col-lg-4 col-md-6 mb-50">
              <div class="footer-widget">
                <div class="footer-widget-heading">
                  <h3>Subscribe now</h3>
                </div>
                <div class="footer-text mb-25">
                  <p>Don't miss to subscribe to our new feeds, kindly fill the form below.</p>
                </div>
                <div class="subscribe-form">
                  <form>
                    <input type="text" placeholder="Email Address">
                    <button type="button"> <v-icon color="white">mdi-send</v-icon></button>
                  </form>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="copyright-area">
        <div class="container">
          <div class="row">
            <div class="col-xl-6 col-lg-6 text-center text-lg-center mx-auto">
              <div class="copyright-text">
                <p>Copyright &copy; 2024 | All Right Reserved | DONUT DISTURB</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </footer>



  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
    };
  },
  mounted() {
    document.addEventListener('contextmenu', this.handleRightClick);

  },
  beforeDestroy() {
    document.removeEventListener('contextmenu', this.handleRightClick);
  },
  methods: {
    handleRightClick(event) {
      event.preventDefault();
    },
    scrollToSection(sectionId) {
      const section = document.querySelector(sectionId);
      if (section) {
        section.scrollIntoView({
          behavior: 'smooth',
          block: 'center', 
        });
      } else {
        console.error('Section not found:', sectionId);
      }
    },
  },
};
</script>





<style>
.animated-button {
  position: relative;
  display: inline-block;
  padding: 12px 24px;
  border: none;
  font-size: 16px;
  font-family: Arial, Helvetica, sans-serif;
  background-color: #612009;
  border-radius: 100px;
  font-weight: 600;
  color: white;
  box-shadow: 0 0 0 2px #612009;
  cursor: pointer;
  overflow: hidden;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1);
  margin-right: 10px;
}

.animated-button span:last-child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 20px;
  height: 20px;
  background-color: #F1F1F1;
  border-radius: 50%;
  opacity: 0;
  transition: all 0.8s cubic-bezier(0.23, 1, 0.320, 1);
}

.animated-button span:first-child {
  position: relative;
  z-index: 1;
}

.animated-button:hover {
  box-shadow: 0 0 0 1px #612009;
  color: #612009;
}

.animated-button:active {
  scale: 0.95;
}

.animated-button:hover span:last-child {
  width: 150px;
  height: 150px;
  opacity: 1;
}


.animated-button-two {
  position: relative;
  display: inline-block;
  padding: 12px 24px;
  border: none;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px;
  background-color: #612009;
  border-radius: 100px;
  font-weight: 600;
  color: white;
  box-shadow: 0 0 0 2px #612009;
  cursor: pointer;
  overflow: hidden;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1);
}

.animated-button-two span:last-child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 20px;
  height: 20px;
  background-color: #F1F1F1;
  border-radius: 50%;
  opacity: 0;
  transition: all 0.8s cubic-bezier(0.23, 1, 0.320, 1);
}

.animated-button-two span:first-child {
  position: relative;
  z-index: 1;
}

.animated-button-two:hover {
  box-shadow: 0 0 0 1px #612009;
  color: #612009;
}

.animated-button-two:active {
  scale: 0.95;
}

.animated-button-two:hover span:last-child {
  width: 150px;
  height: 150px;
  opacity: 1;
}



ul {
  margin: 0px;
  padding: 0px;
  font-family: Arial, Helvetica, sans-serif;
}

.footer-section {
  background: #612009;
  position: relative;
}

.footer-cta {
  border-bottom: 1px solid white;
}

.single-cta i {
  color: #ff5e14;
  font-size: 30px;
  float: left;
  margin-top: 8px;
}

.cta-text {
  padding-left: 15px;
  display: inline-block;

}

.cta-text h4 {
  color: #fff;
  font-size: 20px;
  font-weight: bold;
  font-family: Arial, Helvetica, sans-serif;
  margin-bottom: 2px;

}

.cta-text span {
  color: white;
  font-size: 15px;

}

.footer-content {
  position: relative;
  z-index: 2;
}

.footer-pattern img {
  position: absolute;
  top: 0;
  left: 0;
  height: 330px;
  background-size: cover;
  background-position: 100% 100%;
}

.footer-logo {
  margin-bottom: 30px;
}

.footer-logo img {
  max-width: 200px;
}

.footer-text p {
  margin-bottom: 14px;
  font-size: 14px;
  color: white;
  font-family: Arial, Helvetica, sans-serif;
  line-height: 28px;
}

.footer-social-icon span {
  color: #fff;
  display: block;
  font-size: 20px;
  font-weight: 700;
  font-family: 'Poppins', sans-serif;
  margin-bottom: 20px;
}

.footer-social-icon a {
  color: #fff;
  font-size: 16px;
  margin-right: 15px;
}

.footer-social-icon i {
  height: 40px;
  width: 40px;
  text-align: center;
  line-height: 38px;
  border-radius: 50%;
  margin-left: -10px;
}

.facebook-bg {
  background: #3B5998;
}

.twitter-bg {
  background: #55ACEE;
}

.google-bg {
  background: #DD4B39;
}

.footer-widget-heading h3 {
  color: #fff;
  font-size: 20px;
  font-weight: 600;
  margin-bottom: 40px;
  position: relative;
}

.footer-widget-heading h3::before {
  content: "";
  position: absolute;
  left: 0;
  bottom: -15px;
  height: 2px;
  width: 50px;
  background: white;

}

.footer-widget ul li {
  display: block;
  float: left;
  width: 50%;
  margin-bottom: 12px;
  margin-left: -25px;
}

.footer-widget ul li a:hover {
  color: #ff5e14;
}

.footer-widget ul li a {
  color: white;
  text-transform: capitalize;
}

.subscribe-form {
  position: relative;
  overflow: hidden;
}

.subscribe-form input {
  width: 100%;
  padding: 14px 28px;
  background: white;
  border: 1px solid #2E2E2E;
  color: #fff;
}

.subscribe-form button {
  position: absolute;
  right: 0;
  background: #7b3821;
  padding: 13px 20px;
  border: 1px solid #7b3821;
  top: 0;
}

.subscribe-form button i {
  color: #fff;
  font-size: 22px;
}

.copyright-area {
  background: #7b3821;
  padding: 25px 0;
}

.copyright-text p {
  margin: 0;
  font-size: 14px;
  color: white;
  font-weight: bold;
  font-family: 'Poppins', sans-serif;
}

.copyright-text p a {
  color: #ff5e14;
}

.footer-menu li:hover a {
  color: #ff5e14;
}

.footer-menu li a {
  font-size: 14px;
  color: white;
}</style>