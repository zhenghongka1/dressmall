<template>
  <div class="nav-bar" ignore>
    <div class="left"><slot name="left"></slot></div>
    <div class="center"><slot name="center"></slot></div>
    <div class="right"><slot name="right"></slot></div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style>
.nav-bar {
  display: flex;
  line-height: 3rem;
  height: 3rem;
  box-shadow: 0 1px 1px rgba(100, 100, 100, 0.1);
}

.left,
.right {
  width: 3rem;
}

.center {
  flex: 1;
  text-align: center;
  font-size: 20px;
  /* vertical-align: top; */
}
</style>