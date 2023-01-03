<template>
  <div class="container mt-5 pt-5 pb-5">
    <div class="row">
      <div class="col-lg-6 col-md-6">
        <h4>Based on your reading history</h4>
        <p :style="isDarkMode ? { color: 'white' } : null" class="snippet">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum, in.
          Obcaecati in iusto minima impedit assumenda perferendis natus tempore
          modi ducimus. Blanditiis, quis. Maxime delectus ducimus assumenda vel
          accusantium, eligendi nobis accusamus fuga, hic, natus ab odit. Earum,
          eveniet magnam perspiciatis similique odit cupiditate optio aut fugit,
          inventore, dolorem id?
        </p>
      </div>
      <div class="col-lg-6 col-md-6">
        <img
          src="https://media.istockphoto.com/photos/mobile-responsive-website-development-wireframe-design-preview-on-picture-id844419966?b=1&k=20&m=844419966&s=170667a&w=0&h=Dfps34xqMI2CaLkKMznJnESU4G_XY5evvlC9ui9XEJk="
          alt=""
        />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
const { isDarkMode } = useDarkMode();
</script>
<style scoped>
h4 {
  text-transform: uppercase;
  font-size: 20px;
  color: grey;
}
.snippet {
  margin-top: 30px;
  font-size: 20px;
  line-height: 30px;
}
</style>
