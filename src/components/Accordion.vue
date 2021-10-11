<template>
  <div class="infos">
    <Info
      v-for="(info, i) in infos"
      :info="info"
      :index="i"
      :key="i"
      :open="info.open"
      @toggleOpen="toggleOpen"
    />
  </div>
</template>

<script>
import Info from "./Info.vue";

export default {
  name: "Accordion",
  components: {
    Info,
  },
  data() {
    return {
      infos: [
        {
          client: "Baltimore",
          country: "Estados Unidos",
          contactName: "Lorem Ipsum",
          contactPhone: "+XX XXX XXX XXXX",
          crimeRate: "56.45",
          hero: "The Deep",
          open: false,
        },
        {
          client: "Celaya",
          country: "Mexico",
          contactName: "Lorem Ipsum",
          contactPhone: "+XX XXX XXX XXXX",
          crimeRate: "109.38",
          hero: "A-Train",
          open: false,
        },
        {
          client: "Detroit",
          country: "Estados Unidos",
          contactName: "Lorem Ipsum",
          contactPhone: "+XX XXX XXX XXXX",
          crimeRate: "45.50",
          hero: "Homelander",
          open: false,
        },
        {
          client: "Salvador",
          country: "Brasil",
          contactName: "Lorem Ipsum",
          contactPhone: "+XX XXX XXX XXXX",
          crimeRate: "46.80",
          hero: "Queen Maeve",
          open: false,
        },
        {
          client: "San Pedro Sula",
          country: "Honduras",
          contactName: "Lorem Ipsum",
          contactPhone: "+XX XXX XXX XXXX",
          crimeRate: "41.19",
          hero: "Black Noir",
          open: false,
        },
        {
          client: "Kingston",
          country: "Jamaica",
          contactName: "Lorem Ipsum",
          contactPhone: "+XX XXX XXX XXXX",
          crimeRate: "54.46",
          hero: "Starlight",
          open: false,
        },
        {
          client: "Memphis",
          country: "Estados Unidos",
          contactName: "Lorem Ipsum",
          contactPhone: "+XX XXX XXX XXXX",
          crimeRate: "50.99",
          hero: "Stormfront",
          open: false,
        },
      ],
    };
  },
  methods: {
    toggleOpen: function (index) {
      this.infos = this.infos.map((info, i) => {
        if (index === i) {
          info.open = !info.open;
        } else {
          info.open = false;
        }
        return info;
      });
    },
  },
};
</script>

<style scoped>
.infos {
  padding: 0 10px;
}
</style>        