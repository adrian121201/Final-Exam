<template>
  <div>

    <div style="margin-bottom: 50px; margin-top: 100px;">

      <v-row class="text-center">
        <v-col cols="12">
          <h1 style=" font-family: 'Titan One', sans-serif; font-size: 36px;  color: #612009;">
            Our delightful and quality menu!
          </h1>
        </v-col>
      </v-row>

    </div>

    <div style="margin-bottom: 50px;">
      <v-container>
        <v-row>
          <v-col v-for="(donut, index) in donuts" :key="index" cols="12" sm="6" md="4" lg="3">
            <v-card class="d-flex flex-column align-center elevation-0 card-hover"
              style="background-color: #fff0e8; border-radius: 20px;">
              <v-card-title class="text-center" style="font-family: 'Titan One', sans-serif; color: #612009;">
                {{ donut.title }}
              </v-card-title>
              <v-card-text class="text-center">
                <p style="font-family: Arial, Helvetica, sans-serif; color: #6D4C41;">{{ donut.description }}</p>
              </v-card-text>
              <v-img :src="donut.image" class="image-hover"></v-img>
              <v-card-actions class="d-flex justify-center align-center">
                <v-btn color="white" text style="background-color: #612009; border-radius: 20px; font-size: 12px;">Order
                  Now</v-btn>
                <v-btn icon color="#3E2723">
                  <v-icon>mdi-cart</v-icon>
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>

  </div>
</template>

<script>

export default {
  name: 'ProductPage',
  data() {
    return {
      donuts: [
        {
          title: "Classic Glazed",
          description: "Experience the classic glazed donut with a perfect blend of sweetness.",
          image: require('@/assets/menuone.jpg'),
        },
        {
          title: "Star Fluffy",
          description: "Indulge in the soft and fluffy texture of our star-shaped donut.",
          image: require('@/assets/menutwo.jpg'),
        },
        {
          title: "Rose Filling",
          description: "Delight in the subtle sweetness of our rose-filled donut, the sweetness.",
          image: require('@/assets/menuthree.jpg'),
        },
        {
          title: "Moon",
          description: "Experience the unique taste of our moon-shaped donut well flavor.",
          image: require('@/assets/menufour.jpg'),
        },
        {
          title: "Crown Feeling",
          description: "Feel like royalty with our crown-shaped donut and experienced.",
          image: require('@/assets/menufive.jpg'),
        },
        {
          title: "Dark Glaze",
          description: "Satisfy your cravings with the rich taste of our dark-glazed donut.",
          image: require('@/assets/menusix.jpg'),
        },
        {
          title: "Classic Noble",
          description: "A noble treat with the classic glazed flavor, taste of classic bliss.",
          image: require('@/assets/menuseven.jpg'),
        },
        {
          title: "Classic",
          description: "Indulge in the timeless taste of our classic donut, flavor and classic.",
          image: require('@/assets/menueight.jpg'),
        },
        {
          title: "Circle Feeling",
          description: "Feel like royalty with our crown-shaped donut, get the flavor now.",
          image: require('@/assets/menunine.jpg'),
        },
        {
          title: "Glazed Nuts",
          description: "Satisfy your cravings with the rich taste of our dark-glazed donut.",
          image: require('@/assets/menuten.jpg'),
        },
        {
          title: "Sugar Coated",
          description: "A noble treat with the classic glazed flavor, a glazing flavors and sizes.",
          image: require('@/assets/menueleven.jpg'),
        },
        {
          title: "Twice Feeling",
          description: "Indulge in the timeless taste of our classic donut, feel the twice.",
          image: require('@/assets/menutwelve.jpg'),
        },
      ],
    };
  },
};

</script>

<style>
.card-hover {
  transition: transform 0.1s ease-in-out;
}

.card-hover:hover {
  transform: scale(1.1);
}
</style>