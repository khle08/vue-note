<template>
  <div>
    <p>资料绑定（单向）</p>
    {{ data }}
  </div>

  <div>
    <p>资料绑定（双向）</p>
    <input type="text" v-model="text" />
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>