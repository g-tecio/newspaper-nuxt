<template>
  <b-row>
    <b-col md="4" style=" padding: 10px 20px 20px 10px;">
      <h2>{{ content.title }}</h2>
      <p>
        {{ content.content }}
      </p>

      <img :src="'https://picsum.photos/1024/400/?image=' + content.img" alt="Avatar" class="avatar">
      <p style="display: inline-block">by Steven Voorhees</p>
      <br>
      <div class="left_section">
        <span class="city">Thuesday, February 2</span>
        <img src="./icons/fb.png" class="icons" alt>
        <img src="./icons/li.png" class="icons" alt>
        <img src="./icons/tw.png" class="icons" alt>
        <img src="./icons/yt.png" class="icons" alt>
      </div>
    </b-col>
    <b-col md="8">
      <b-img
        :src="'https://picsum.photos/1024/400/?image=' + content.img"
        fluid-grow
        alt="Fluid-grow image"
        style="max-width: 100%; height: auto;"
      />
    </b-col>
  </b-row>
</template>
<script>
export default {
  props: ['content']
};
</script>
