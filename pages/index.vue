<template>
  <div>
    <Hero />
    <Signature />
    <TheHouseBlend />
    <Medium />
    <News />
  </div>
</template>

<script>
import Hero from '../components/Hero.vue';
import Signature from '../components/Signature.vue';
import TheHouseBlend from '../components/HouseBlend.vue';
import Medium from '../components/Medium.vue';
import News from '../components/News.vue';

export default {
  components: {
    Hero,
    Signature,
    TheHouseBlend,
    Medium,
    News,
  }
}
</script>
