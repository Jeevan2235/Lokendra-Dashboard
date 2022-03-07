<template>
  <div>
    <v-row justify="center" class="mt-16">
      <v-card width="47em" class="pa-5">
        <v-row>
          <v-col cols="12" md="2">
            <v-card-text class="font-weight-bold">Full Name</v-card-text>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field solo></v-text-field>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" md="2">
            <v-card-text class="font-weight-bold">Contact</v-card-text>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field solo></v-text-field>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" md="2">
            <v-card-text class="font-weight-bold">E-mail</v-card-text>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field solo></v-text-field>
          </v-col>
        </v-row>
        <v-row>
          <v-col cols="12" md="2">
            <v-card-text class="font-weight-bold">Address</v-card-text>
          </v-col>
          <v-col cols="12" md="6">
            <v-text-field solo></v-text-field>
            <v-row justify="center">
              <v-btn
                class="mt-3 mb-10 white--text"
                color="#f94f19"
                rounded
                elevation="0"
                height="2.5em"
                width="9em"
              >
                Save</v-btn
              >
            </v-row>
          </v-col>
        </v-row>
      </v-card>
    </v-row>
  </div>
</template>

<script>
export default {};
</script>

<style></style>
