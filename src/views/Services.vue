<template>
  <div class="content">
    <div class="layout layout--style-a">
      <div class="layout__inner">
        <Title main="Services" />
        <Contracting />
        <Websites />
      </div>
    </div>
  </div>
</template>

<script>
import Title from "@/components/title/Title.vue";
import Contracting from "@/components/contracting/Contracting.vue";
import Websites from "@/components/websites/Websites.vue";

export default {
  name: "services",
  components: {
    Contracting,
    Websites,
    Title
  }
};
</script>
