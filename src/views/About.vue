<template>
  <v-container>
    <v-row>
      <v-col cols="3">Prvi stupac</v-col>
      <v-col cols="4">Drugi stupac</v-col>
      <v-col cols="5">Treći stupac</v-col>
    </v-row>

    <v-row>
      <v-col v-for="broj in 6" :key="broj"> {{ broj }}. stupac </v-col>
    </v-row>

    <v-row>
      <v-col v-for="broj in 3" :key="broj">
        <v-card class="mx-auto" max-width="344" outlined>
          <v-list-item three-line>
            <v-list-item-content>
              <div class="overline mb-4">OVERLINE</div>
              <v-list-item-title class="headline mb-1">
                Headline 5
              </v-list-item-title>
              <v-list-item-subtitle
                >Greyhound divisely hello coldly
                fonwderfully</v-list-item-subtitle
              >
            </v-list-item-content>

            <v-list-item-avatar
              tile
              size="80"
              color="grey"
            ></v-list-item-avatar>
          </v-list-item>

          <v-card-actions>
            <v-btn outlined rounded text> Button </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
