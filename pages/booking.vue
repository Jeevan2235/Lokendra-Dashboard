<template>
  <div>
    <v-col md="11">
      <v-card class="mt-5" tile outlined v-for="link in links" :key="link">
        <v-row>
          <v-col md="2" cols="12">
            <v-img class="ma-2 mt-4" :src="link.img"></v-img>
          </v-col>
          <v-col class="ma-5" md="7" cols="12">
            <p style="line-height: 10px">{{ link.name }}</p>
            <p style="line-height: 10px">{{ link.sport }}</p>
            <p style="line-height: 10px">{{ link.date }}</p>
            <p style="line-height: 10px">{{ link.time }}</p>
          </v-col>
          <v-col md="2" cols="12">
            <v-btn class="my-3" tile elevation="1">Book Now</v-btn>
            <v-btn tile elevation="1">Cancel</v-btn>
          </v-col>
        </v-row>
      </v-card>
    </v-col>
  </div>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          img: "1.jpg",
          name: "Name: Lokendra Thapa",
          sport: " Sport: Basketball",
          date: "Date: 11/11/2020",
          time: " Time: 7am - 8am",
        },
        {
          img: "4.png",
          name: "Name: Jeevan Shrestha",
          sport: " Sport: Futsal",
          date: "Date: 11/11/2020",
          time: " Time: 10am - 12am",
        },
        {
          img: "3.png",
          name: "Name: Sushan Shakya",
          sport: " Sport: Badminton",
          date: "Date: 11/11/2020",
          time: " Time: 5am - 8am",
        },
        {
          img: "2.jpg",
          name: "Name: Dipesh Shakya",
          sport: " Sport: Volleyball",
          date: "Date: 11/11/2020",
          time: " Time: 5am - 6pm",
        },
      ],
    };
  },
};
</script>
