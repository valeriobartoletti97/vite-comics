<template>
  <div class="my-card">
        <div class="img-box">
            <img :src="img" :alt="title">
        </div>
        <h5 class="text-uppercase pt-3">
            {{title}}
        </h5>
    </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    img: String,
    title: String,
    alt: String,
  },
};
</script>

<style lang="scss">
.my-card{
  width: 200px;
  .img-box {
    width: 200px;
    height: 200px;
    overflow: hidden;
    cursor: pointer;
    img{
        object-fit: contain;
        width: 100%
    }
  }
  h5{
        color: white;
        font-size: 1.4em;
        font-weight: 700
    }
}
</style>
