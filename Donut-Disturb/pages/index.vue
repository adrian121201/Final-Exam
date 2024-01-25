<template>
  <div>

    <div style="margin-top: 50px;">
      <v-container fluid fill-height class="pa-0">
        <v-row no-gutters>
          <v-col>
            <v-img :src="require('@/assets/introWallpaper.jpg')">
              <v-container style="margin-top: 20vh;">
                <v-row>
                  <v-col cols="12" class="text-left">
                    <h1
                      style="margin-bottom: 20px; max-width: 400px; font-family: 'Titan One', sans-serif; color: #612009;">
                      Discover Our Delicious Donuts Today!</h1>
                    <p style="max-width: 600px; color: #6D4C41; font-family: Arial, Helvetica, sans-serif;">
                      We believe in turning ordinary moments into extraordinary memories, one delectable donut at a time.
                      Step into a world where the aroma of freshly baked goodness fills the air, and every bite is a
                      journey into a realm of pure delight.
                    </p>
                  </v-col>
                  <v-col cols="12" class="text-left">

                    <button class="animated-button">
                      <span>See more</span>
                      <span></span>
                    </button>

                    <router-link to="/products">

                      <button class="animated-button-two">
                        <span>Our menu</span>
                        <span></span>
                      </button>

                    </router-link>

                  </v-col>
                </v-row>
              </v-container>
            </v-img>
          </v-col>
        </v-row>
      </v-container>
    </div>


    <div style="margin-top: 50px; margin-bottom: 100px;">
      <v-container>
        <v-row align="center">
          <v-col v-for="card in cards" :key="card.title" cols="12" md="6" lg="3">
            <v-card class="pa-3 text-center elevation-0"
              style="border-radius: 15px; background-color: #fff0e8; display: flex; flex-direction: column; align-items: center;">
              <v-btn class="elevation-0" style="border-radius: 50%; background-color: white; height: 80px;">
                <v-icon color="#612009" class="display-2 mb-2" style="font-size: 3em;">{{ card.icon }}</v-icon>
              </v-btn>
              <v-card-title style="margin-top: 10px; font-family: 'Titan One', sans-serif; color: #612009;">{{ card.title
              }}</v-card-title>
              <v-card-subtitle style="margin-top: 10px; color: #6D4C41;">{{ card.subtext }}</v-card-subtitle>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>

    <div style="margin-bottom: 100px;" id="our-story">
      <v-container>
        <v-card class="mt-5 text-center elevation-0" color="transparent">
          <v-row align="center" class="mx-auto" style="max-width: 100%;">
            <v-col cols="12" md="4">
              <v-img :src="require('@/assets/donut-story.png')" alt="About Us Image" height="380px" width="600px"
                style="border-radius: 40px;"></v-img>
            </v-col>
            <v-col cols="12" md="8">
              <v-card-title style="font-family: 'Titan One', sans-serif; color: #612009; font-size: 40px;">A brief of our
                lovely story</v-card-title>
              <v-card-text
                style="font-family: Arial, Helvetica, sans-serif; color:#6D4C41; max-width: 700px; text-align: justify; line-height: 28px; display: flex; flex-direction: column;">
                Savor the joy of delightful donuts at Donut Delight - your go-to destination for indulgent, mouth-watering
                treats. Our commitment to sweetness and unwavering dedication to quality have made us the top choice for
                discerning individuals who crave the perfect blend of flavor, texture, and satisfaction.
                <v-row>

                  <button class="animated-button-about">
                    <span>About us</span>
                    <span></span>
                  </button>

                </v-row>
              </v-card-text>
            </v-col>
          </v-row>
        </v-card>
      </v-container>
    </div>


    <div style="margin-bottom: 100px;">
      <v-container>
        <v-card class="mt-5 text-center elevation-0" color="transparent">
          <v-row align="center" class="mx-auto" style="max-width: 100%;">
            <v-col cols="12" md="8">
              <v-card-title style="font-family: 'Titan One', sans-serif; color: #612009; font-size: 40px;">Our delightful
                menu for you!</v-card-title>
              <v-card-text
                style="font-family: Arial, Helvetica, sans-serif; color:#6D4C41; max-width: 700px; text-align: justify; line-height: 28px; display: flex; flex-direction: column;">
                Embark on a culinary journey with our delectable menu at Donut Delight. Indulge your senses in a symphony
                of flavors crafted to perfection. From classic favorites to innovative delights, our menu is a celebration
                of sweet sensations.
                <v-row>
                  <router-link to="/products">
                    <button class="animated-button-menu">
                      <span>Our menu</span>
                      <span></span>
                    </button>
                  </router-link>
                </v-row>
              </v-card-text>
            </v-col>
            <v-col cols="12" md="4">
              <v-img :src="require('@/assets/menu-donut.jpg')" alt="About Us Image" height="380px" width="600px"
                style="border-radius: 40px;"></v-img>
            </v-col>
          </v-row>
        </v-card>
      </v-container>
    </div>


    <div style="margin-bottom: 100px;">
      <v-container fluid class="pa-0">
        <v-row>
          <v-col cols="12" class="p-0">
            <div style="position: relative;">
              <v-img :src="require('@/assets/offer-donut.jpg')" alt="Long Picture" class="d-flex align-center"
                style="width: 100%; height: 500px; position: relative;">
                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-col cols="12" class="text-center">
                    <div style="max-width: 800px; margin: auto;">
                      <v-card color="transparent" class="white--text elevation-0">
                        <v-card-text
                          style="font-family: Arial, Helvetica, sans-serif; font-size: 30px; font-weight: bold; color: #612009;">
                          Get our offer!
                        </v-card-text>
                        <v-card-subtitle
                          style="font-family: 'Titan One', sans-serif; color: #612009; font-size: 35px; line-height: 40px;">
                          Connect with us and get 35% off to our all products
                        </v-card-subtitle>
                      </v-card>
                    </div>
                  </v-col>
                </v-row>

                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-col cols="12" class="text-center">
                    <button class="animated-button-getnow">
                      <span>Get now</span>
                      <span></span>
                    </button>
                  </v-col>
                </v-row>
              </v-img>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>



    <div style="margin-bottom: 100px; background-color: #fff0e8; height: auto;" id="reviews">
      <div>
        <v-row class="text-center">
          <v-col cols="12">
            <h1 style="font-family: 'Titan One', sans-serif; font-size: 36px; color: #612009; margin-top: 40px;">
              Let's hear out our donut speakers
            </h1>
          </v-col>
        </v-row>
      </div>

      <v-container>
        <v-carousel cycle hide-delimiters>
          <v-carousel-item v-for="(item, index) in chunkedReviewsItems" :key="index">

            <v-row justify="center" align="center">
              <v-col v-for="(review, reviewIndex) in item" :key="reviewIndex" cols="12" sm="4">
                <v-card class="mx-auto elevation-0" color="white" dark max-width="400" max-height="400"
                  style="border-radius: 20px; margin-top: 90px;">


                  <v-card-title style="color: black;">
                    <span style="font-family: Arial, Helvetica, sans-serif; font-size: 15px; color: black;">Reviews</span>
                  </v-card-title>

                  <v-list-item>
                    <v-list-item-avatar color="grey darken-3">
                      <v-img class="elevation-6" alt="" :src="review.picture"></v-img>
                    </v-list-item-avatar>

                    <v-list-item-content>
                      <v-list-item-title style="color: rgb(85, 85, 85);">{{ review.name }}</v-list-item-title>
                    </v-list-item-content>
                  </v-list-item>

                  <v-card-text class="text-h7 font-weight-bold" style="color: black"> "{{ review.text }}" </v-card-text>

                  <v-rating v-model="review.rating" background-color="transparent" color="yellow" dense half-increments
                    readonly style="margin-left: 10px;"></v-rating>

                  <v-card-actions>
                    <v-row align="center" justify="space-between" class="w-100">
                      <v-col>
                        <v-icon class="mr-1" style="color: black;">mdi-Like</v-icon>
                        <span class="subheading" style="color: black;">{{ review.shares }}</span>
                      </v-col>
                    </v-row>
                  </v-card-actions>
                </v-card>
              </v-col>
            </v-row>
          </v-carousel-item>
        </v-carousel>
      </v-container>
    </div>




    <div id="contact-us" style="margin-bottom: 100px;">
      <v-container fluid class="pa-0">
        <v-row class="fill-height ma-0" align="center" justify="center">
          <v-col cols="12" class="pa-0 text-center">
            <div style="position: relative;">
              <v-img :src="require('@/assets/contactus-donut.jpg')" alt="Long Picture" class="d-flex align-center"
                style="width: 100%; height: 500px; position: relative;">

                <div
                  style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; background-color: rgba(0, 0, 0, 0.5);">
                </div>

                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-col cols="12">
                    <div style="max-width: 800px; margin: auto;">
                      <v-card color="transparent" class="white--text elevation-0">
                        <v-card-text
                          style="font-family: 'Titan One', sans-serif; color: white; font-size: 35px; line-height: 40px;">
                          Contact us and join our community, and stay up to date.
                        </v-card-text>
                        <v-card-subtitle
                          style="font-family: Arial, Helvetica, sans-serif; color: white; font-size: 15px;">
                          You'll be the first to know about new flavors, seasonal specials, and limited-time offers.
                        </v-card-subtitle>
                      </v-card>
                    </div>
                  </v-col>
                </v-row>

                <v-row class="fill-height ma-0" align="center" justify="center">
                  <v-col cols="12">
                    <v-text-field label="Enter your email" solo clearable
                      style="width: 500px; margin: auto; border-radius: 20px; font-family: Arial, Helvetica, sans-serif; font-size: 13px; font-weight: bold;"
                      class="elevation-0">
                      <template v-slot:append>
                        <v-btn class="elevation-0"
                          style="background-color: #612009; width: 100px; border-radius: 20px; height: 40px;">
                          <v-icon color="white">mdi-send</v-icon>
                        </v-btn>
                      </template>
                    </v-text-field>
                  </v-col>
                </v-row>
              </v-img>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>




  </div>
</template>

<style>
.animated-button-about {
  position: relative;
  display: inline-block;
  padding: 12px 24px;
  border: none;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px;
  background-color: white;
  border-radius: 100px;
  font-weight: 600;
  color: #612009;
  box-shadow: 0 0 0 1px #612009;
  cursor: pointer;
  overflow: hidden;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1);
  margin-top: 30px;
  margin-left: 10px;
}

.animated-button-about span:last-child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 20px;
  height: 20px;
  background-color: #612009;
  border-radius: 50%;
  opacity: 0;
  transition: all 0.8s cubic-bezier(0.23, 1, 0.320, 1);
}

.animated-button-about span:first-child {
  position: relative;
  z-index: 1;
}

.animated-button-about:hover {
  box-shadow: 0 0 0 1px #612009;
  color: white;
}

.animated-button-about:active {
  scale: 0.95;
}

.animated-button-about:hover span:last-child {
  width: 150px;
  height: 150px;
  opacity: 1;
}



.animated-button-menu {
  position: relative;
  display: inline-block;
  padding: 12px 24px;
  border: none;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px;
  background-color: white;
  border-radius: 100px;
  font-weight: 600;
  color: #612009;
  box-shadow: 0 0 0 1px #612009;
  cursor: pointer;
  overflow: hidden;
  transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1);
  margin-top: 30px;
  margin-left: 10px;
}

.animated-button-menu span:last-child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 20px;
  height: 20px;
  background-color: #612009;
  border-radius: 50%;
  opacity: 0;
  transition: all 0.8s cubic-bezier(0.23, 1, 0.320, 1);
}

.animated-button-menu span:first-child {
  position: relative;
  z-index: 1;
}

.animated-button-menu:hover {
  box-shadow: 0 0 0 1px #612009;
  color: white;
}

.animated-button-menu:active {
  scale: 0.95;
}

.animated-button-menu:hover span:last-child {
  width: 150px;
  height: 150px;
  opacity: 1;
}



.animated-button-getnow {
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
  margin-top: 30px;
  margin-left: 10px;
}

.animated-button-getnow span:last-child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 20px;
  height: 20px;
  background-color: white;
  border-radius: 50%;
  opacity: 0;
  transition: all 0.8s cubic-bezier(0.23, 1, 0.320, 1);
}

.animated-button-getnow span:first-child {
  position: relative;
  z-index: 1;
}

.animated-button-getnow:hover {
  box-shadow: 0 0 0 1px #612009;
  color: #612009;
}

.animated-button-getnow:active {
  scale: 0.95;
}

.animated-button-getnow:hover span:last-child {
  width: 150px;
  height: 150px;
  opacity: 1;
}
</style>


<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      cards: [
        { icon: 'mdi-motorbike', title: 'Fast Delivery', subtext: 'Get your donuts delivered in record time. Our fast and efficient delivery ensures you enjoy your treats without waiting.' },
        { icon: 'mdi-check', title: 'Best Quality', subtext: 'Indulge in the highest quality ingredients. We source only the finest components to create our delicious and satisfying donuts.' },
        { icon: 'mdi-chef-hat', title: 'Quality Taste', subtext: 'Experience a symphony of flavors with our donuts. Each bite is a journey into a realm of taste, sweetness perfection.' },
        { icon: 'mdi-star', title: 'All Time Best', subtext: 'Discover our customer favorites. Our all-time bestsellers are crafted to perfection, ensuring a delightful experience.' },
      ],
      reviewsItems: [
        {
          text: "Absolutely loved the donuts! They were incredibly fresh and flavorful. I can't get enough of them! Highly recommend trying them out!",
          picture: 'https://www.billboard.com/wp-content/uploads/2022/05/nayeon-twice-2022-press-billboard-1548.png',
          name: '@nayeon',
          rating: 5,
        },
        {
          text: "These donuts are divine! The variety of flavors is impressive, and they simply melt in your mouth. You won't be disappointed!",
          picture: 'https://6.soompi.io/wp-content/uploads/image/20230728152120_Jihyo-2.jpg?s=900x600&e=t',
          name: '@jihyo',
          rating: 5,
        },
        {
          text: "Amazing donuts! The texture and taste are outstanding. Each bite feels like a little piece of heaven. Can't wait to visit again!",
          picture: 'https://qph.cf2.quoracdn.net/main-qimg-a6b8a6bf79bc0780cf1cc7f4ca5c0e77-lq',
          name: '@momo',
          rating: 5,
        },
        {
          text: "I'm in love with these donuts! The flavors are simply amazing, and they're always so fresh and scrumptious!",
          picture: 'https://image-cdn.hypb.st/https%3A%2F%2Fhypebeast.com%2Fwp-content%2Fblogs.dir%2F6%2Ffiles%2F2022%2F10%2Fgucci-newjeans-hanni-brand-ambassdaor-announcement-tw.jpg?w=960&cbr=1&q=90&fit=max',
          name: '@hanni',
          rating: 5,
        },
        {
          text: "I'm obsessed with these donuts! The freshness and flavors are top-notch. A must-try for any donut enthusiast!",
          picture: 'https://image.kpopmap.com/2023/06/NewJeans-MinJi-W-Korea.jpg',
          name: '@minji',
          rating: 5,
        },
        {
          text: "These donuts are pure bliss! The flavors are so rich and delightful. You won't regret indulging in these heavenly treats!",
          picture: 'https://assets.puzzlefactory.com/puzzle/520/361/original.jpg',
          name: '@haerin',
          rating: 5,
        },
        {
          text: "These donuts are pure ecstasy! The flavors are so sumptuous and delightful. Indulging in these heavenly treats is a decision you won't regret!",
          picture: 'https://image.kpopmap.com/2019/01/ITZY-RyuJin-070522.jpg',
          name: '@ryujin',
          rating: 5,
        },
        {
          text: "These donuts are pure bliss! The flavors are so rich and delightful. You won't regret indulging in these heavenly treats!",
          picture: 'https://static.promediateknologi.id/crop/0x428:1536x1565/750x500/webp/photo/2023/02/20/20230220_130415-4102120673.jpg',
          name: '@jiwon',
          rating: 5,
        },
        {
          text: "Donuts delivering sheer bliss! The flavors are exceptionally rich and delightful. Treating yourself to these heavenly flavors",
          picture: 'https://unnielooks.com/cdn/shop/articles/FLTGsPwVcAA_PZR.jpg?v=1655895737&width=1100',
          name: '@sana',
          rating: 5,
        },
        {
          text: "Indulge in these blissful donuts! The flavors offer a decadently rich and delightful experience. This is a truly worth!",
          picture: 'https://6.soompi.io/wp-content/uploads/image/b036a9dfce614a24a93919cd5eed5676.jpeg?s=900x600&e=t',
          name: '@lisa',
          rating: 5,
        },
      ],
    };
  },
  computed: {
    chunkedReviewsItems() {

      const chunkSize = 2;
      return this.reviewsItems.reduce((resultArray, item, index) => {
        const chunkIndex = Math.floor(index / chunkSize);

        if (!resultArray[chunkIndex]) {
          resultArray[chunkIndex] = [];
        }

        resultArray[chunkIndex].push(item);

        return resultArray;
      }, []);
    },
  },
};
</script>
