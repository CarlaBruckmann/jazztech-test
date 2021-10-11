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

         