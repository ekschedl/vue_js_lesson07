<template>
  <div>
    <div class="circle circle-big">
      <div class="circle circle-mini">
        <button>click</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.circle {
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50%;

  &-big {
    width: 200px;
    height: 200px;
    background-color: red;
  }

  &-mini {
    width: 150px;
    height: 150px;
    background-color: green;
  }
}
</style>