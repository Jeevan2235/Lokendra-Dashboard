<template>
<v-card class="pa-10" elevation="0"> 
    <v-simple-table fixed-header height="350px">
    <template v-slot:default>
      <thead>
        <tr>
          <th class="text-left">Name</th>
          <th class="text-left">Phone Number</th>
          <th class="text-left">E-mail</th>
          <th class="text-left">User ID</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in desserts" :key="item.name">
          <td>{{ item.name }}</td>
          <td>{{ item.phonenumber }}</td>
          <td>{{ item.email }}</td>
          <td>{{ item.id }}</td>
        </tr>
      </tbody>
    </template>
  </v-simple-table>
</v-card>
</template>
]

<script>
export default {
  data() {
    return {
      desserts: [
        {
          name: "Frozen Yogurt",
          phonenumber: 159,
          email: "abc@gmail.com",
          id: "10",
        },
        {
          name: "Frozen Yogurt",
          phonenumber: 159,
          email: "abc@gmail.com",
          id: "10",
        },
        {
          name: "Frozen Yogurt",
          phonenumber: 159,
          email: "abc@gmail.com",
          id: "10",
        },
        {
          name: "Frozen Yogurt",
          phonenumber: 159,
          email: "abc@gmail.com",
          id: "10",
        },
        {
          name: "Frozen Yogurt",
          phonenumber: 159,
          email: "abc@gmail.com",
          id: "10",
        },
        {
          name: "Frozen Yogurt",
          phonenumber: 159,
          email: "abc@gmail.com",
          id: "10",
        },
      ],
    };
  },
};
</script>
