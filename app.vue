<template>
  <div class="">
  <div class="  py-4 bg-img ">
  <div class="">
    <Navi/>
  </div>
  <Hero/>
</div>
<Trust/>
  </div>
</template>
<script>
export default {
  data() {
    return {
      menuOpen: false,
    };
  },
};  

</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
.bg-img{
  background-image: linear-gradient(134deg, #0C0091 0%, #00A87E 100%);;
}
*{
  font-family: 'Poppins', sans-serif;
}
.transition-transform {
  transition-property: transform;
}
.transform {
  transform-origin: center;
}
.transform-rotate-180 {
  transform: rotate(180deg);
}
</style>
