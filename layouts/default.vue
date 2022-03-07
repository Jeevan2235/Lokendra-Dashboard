<template>
  <v-app>
    <v-navigation-drawer v-model="drawer" dark app class="pink accent-4">
       <v-row class="mt-1" justify="center">
            <v-icon size="130">mdi-account</v-icon>
          </v-row>
            <v-divider class="mt-3"></v-divider>
      <v-list flat class="mt-10">
        <v-list-item
          v-for="link in links"
          :key="link"
          router
          :to="link.route"
          active-class="border"
        >
          <v-list-item-action>
            <v-icon>{{link.icon}}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>{{link.title}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <template v-slot:append>
            <div class="pa-2">
              <v-btn block> Log out </v-btn>
            </div>
          </template>
    </v-navigation-drawer>
    <v-main>
      <Nuxt />
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      links: [
        { title: "Booking", icon: "mdi-view-dashboard", route:"/booking" },
        { title: "User", icon: "mdi-account-box", route:"/user" },
        { title: "My Profile", icon: "mdi-gavel", route:"/profile" },
      ],
    };
  },
};
</script>

<style></style>
