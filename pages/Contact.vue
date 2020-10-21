<template>
  <v-card
    class="mx-auto"
    max-width="500"
  >


    <v-container fluid>
      <v-row dense>
        <v-col
          v-for="card in cards"
          :key="card.title"
          :cols="card.flex"
        >
          <v-card>
            <v-img
              :src="card.src"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
            >
              <v-card-title v-text="card.title"></v-card-title>
            </v-img>

            <v-card-actions>
              <v-spacer></v-spacer>

              <v-btn icon>
                <v-icon>mdi-heart</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-bookmark</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-share-variant</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>
<script>
  export default {
    name: 'contact',
    data: () => ({
        
cards: [
{
'id': 1,
title: 'Morty',
src: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg',
flex: 6
},
{
'id': 2,
title: 'Rick',
src: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg',
flex: 6
},
{
id: 3,
title: 'Summer',
src: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg',
flex: 6
},
{
id: 4,
title: 'Beth',
src: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg',
flex: 6
},
{
id: 5,
title: 'Jerry',
src: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg',
flex: 6
}
],
    }),
  }
</script>

      cards: [
        { title: 'Pre-fab homes', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 12 },
        { title: 'Favorite road trips', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 6 },
        { title: 'Best airlines', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg',  },
      ],