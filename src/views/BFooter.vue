<template>
  <v-footer dark padless>
    <v-card class="flex" flat tile>
      <v-card-title class="teal">
        <strong class="subheading"
          >Lorem ipsum dolor sit amet consectetur, adipisicing elit.</strong
        >

        <v-spacer></v-spacer>

        <v-btn v-for="icon in icons" :key="icon" class="mx-4" dark icon>
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 white--text text-center">
        {{ new Date().getFullYear() }}
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  name: "BFooter",
  data: () => ({
    icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
  }),
};
</script>

<style></style>
