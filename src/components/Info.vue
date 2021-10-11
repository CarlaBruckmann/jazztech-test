<template>
  <div :class="open ? 'info open' : 'info'" @click="$emit('toggleOpen', index)">
    <div class="client title-accordion">{{ info.client }}</div>
    <div class="country info-accordion">País: {{ info.country }}</div>
    <div class="contactName info-accordion">
      Contato: {{ info.contactName }}
    </div>
    <div class="contactPhone info-accordion">
      Telefone: {{ info.contactPhone }}
    </div>
    <div class="crimeRate info-accordion">
      Indice de Criminalidade: {{ info.crimeRate }}
    </div>
    <div class="hero info-accordion">Herói Indicado: {{ info.hero }}</div>
  </div>
</template>

<script>
export default {
  name: "Info",
  props: ["info", "index", "open"],
};
</script>

<style >
.info {
  width: 100%;
  margin: 30px 0;
}
.info .title-accordion {
  width: 100%;
  padding: 10px;
  transition: all 0.4 linear;
  font-family: var(--font-primary);
  font-size: 18px;
  position: relative;
  background-color: var(--blue-accent);
  cursor: pointer;
}
.info .title-accordion::after {
  content: "";
  position: absolute;
  top: 50%;
  right: 0;
  margin: 0 20px;
  transform: translateY(-50%) rotate(0deg);
  width: 15px;
  height: 15px;
  background-image: url("./assets/arrow.svg");
  background-position: center;
  background-size: content;
  background-repeat: no-repeat;
  transition: all 0.2s linear;
}
.info .info-accordion {
  padding: 10px 20px;
  font-family: var(--font-secundary);
  font-size: 14px;
  overflow-y: hidden;
  transition: all 0.4s ease-out;
  display: none;
}
.info.open {
  background-color: var(--white);
}
.info.open .info-accordion {
  display: block;
}
.info.open .title-accordion::after {
  transform: translateY(-50%) rotate(90deg);
}
</style>  