<template>
  <v-app>
    <v-main>
      <v-container class="px-10 mt-m2" fluid>
        <v-carousel height="100%" cycle :interval="2000" hide-delimiters>
          <v-carousel-item class="bg-light-white text-center">
            <v-row dense>
              <v-col v-for="(variant, i) in variants" :key="i" cols="12" sm="4">
                <v-card
                  :variant="variant"
                  color="#757575"
                  theme="dark"
                  class="rounded-xl"
                  height="285"
                >
                  <div class="d-flex flex-no-wrap justify-space-between">
                    <div>
                      <v-card-title class="text-h4 mt-10">
                        KSM BEDAH
                      </v-card-title>
                      <v-card-subtitle> Jadwal </v-card-subtitle>
                    </div>
                    <v-img
                      src="~/assets/1.png"
                      class="mr-4 mt-5"
                      absolute
                    ></v-img>
                  </div>
                </v-card>
              </v-col>
            </v-row>
          </v-carousel-item>
          <v-carousel-item class="bg-light-white text-center">
            <v-row dense>
              <v-col v-for="(variant, i) in variants" :key="i" cols="12" sm="4">
                <v-card
                  color="variant"
                  theme="dark"
                  class="rounded-xl"
                  height="285"
                >
                  <div class="d-flex flex-no-wrap justify-space-between">
                    <div>
                      <v-card-title class="text-h4 mt-10">
                        KSM BEDAH
                      </v-card-title>
                      <v-card-subtitle> Jadwal </v-card-subtitle>
                    </div>
                    <v-img
                      src="~/assets/1.png"
                      class="mr-4 mt-5"
                      absolute
                    ></v-img>
                  </div>
                </v-card>
              </v-col>
            </v-row>
          </v-carousel-item>
        </v-carousel>
      </v-container>
    </v-main>
  </v-app>
</template>
<script>
export default {
  data: () => ({
    variants: ["elevated", "flat", "tonal", "outlined", "text", "plain"],
  }),
};
</script>
