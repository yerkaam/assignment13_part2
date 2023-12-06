<template>
  <div id="app" class="app">
    <app-accordion class="accordion">
      <template v-slot:title>
        <span class="text">Accordion 1</span>
      </template>
      <template v-slot:content>
        <p>
          <b>Lorem</b>, ipsum dolor sit amet consectetur adipisicing elit. Quia,
          porro. Non a excepturi, voluptatibus ipsam magnam, eligendi,
          accusantium ipsa quae quis praesentium voluptate saepe ullam sint ea
          itaque consectetur impedit?
        </p>
      </template>
    </app-accordion>

    <app-accordion class="accordion">
      <template v-slot:title>
        <span class="text">Accordion 2</span>
      </template>
      <template v-slot:content>
        <p>
          <b>Lorem</b>, ipsum dolor sit amet consectetur adipisicing elit. Quia,
          porro. Non a excepturi, voluptatibus ipsam magnam, eligendi,
          accusantium ipsa quae quis praesentium voluptate saepe ullam sint ea
          itaque consectetur impedit?
        </p>
      </template>
    </app-accordion>
  </div>
</template>

<script>
import AppAccordion from "./components/AppAccordion.vue";

export default {
  name: "App",
  components: {
    AppAccordion,
  },
};
</script>

<style>
.app{
  padding:15px;
}
.accordion{
  margin-bottom: 30px;
}
.text{
  font-size: 1.25em;
  font-weight: 600;
}
</style>