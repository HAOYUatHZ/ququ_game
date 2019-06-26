<template>
  <div class="is-marginless text-center" >
    <h1 class="home-h" style="margin-top:180px;">欢迎来到"宛渠之民"</h1>
    <h1 class="home-h" style="margin-top:40px;">2019.6.26</h1>
  </div>
</template>

<script>
import { Slider, SliderItem } from 'vue-easy-slider';

export default {
  name: 'PackViewNew',
  components: {
    Slider,
    SliderItem
  },
  data() {
    return {};
  },
  methods: {}
};
</script>

<style scoped>
.text-center{
  text-align: center;
}
.home-h {
  font-size: 40px;
  font-weight: bold;
  color: white;
  text-shadow:2px 2px 5px #333333;
}
</style>
