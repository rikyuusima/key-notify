<template>
  <section>
    <h2>{{section_name}}</h2>
    <slot></slot>
  </section>
</template>

<script>
  export default {
    props: ['section_name']
  }
</script>

<style lang="less" scoped>
  @import "../less/main.less";

  section{
    background-color: @article-back-color;
    width: @content-small-size;
    height: auto;

    .screen-sm({
      width: 45vw;
      flex-direction: row;
    });

    .screen-md({
      width: 45vw;
      flex-direction: row;
    });

    .screen-lg({
      width: 45vw;
      flex-direction: row;
    });
  }

  h2{
    margin: 0;
    margin-bottom: 10px;
    background-color: @title-back-color;
    padding-left: 1vw;
    font-weight: normal;
    font-style: normal;
    font-size: 1rem;
  }
</style>

