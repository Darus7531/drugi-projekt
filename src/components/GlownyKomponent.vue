<template>
  <div class="Card">
    <div class="Card-description">
      <img
        class="Card-profile"
        src="https://sites.google.com/site/cherryblossom3182015/_/rsrc/1436359773127/comments/yiruma-161010.jpg"
        alt="tutaj powinno być zdjęcie"
      />

      <h2>{{ title }}<br /></h2>
      {{ description }}
    </div>
    <div class="Card-photo"><Photo /></div>
  </div>
</template>
<script>
import Photo from "./Photo";

export default {
  name: "GlownyKomponent",
  components: {
    Photo,
  },
  data() {
    return {
      title: "Yiruma",
      description:
        "Południowokoreański pianista i kompozytor. Yiruma występował na koncertach w Azji, Europie i Ameryce Północnej. Jego Alma Mater, King’s College London, pomogła mu zdobyć popularność w Europie. Wśród jego utworów najbardziej popularne są „River Flows in You”, „Kiss the Rain” i „May Be”.",
    };
  },
};
</script>
<style>
.Card {
  width: 1035px;
  height: 500px;
  background-color: #f0f0f0;
  margin: auto;
  border: 5px solid #000;
  display: flex;
}

.Card-profile {
  border-radius: 50%;
  width: 190px;
  height: 150px;
}
.Card-description {
  width: 210px;
  height: 100px;
  margin: 30px;
}
</style>
