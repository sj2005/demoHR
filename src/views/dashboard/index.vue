<template>
  <div class="dashboard-container">
    <div class="dashboard-text">name: {{ name }}</div>
    <!-- svg-icon使用練習 -->
    <svg-icon icon-class="dashboard"></svg-icon>
    <svg-icon icon-class="example"></svg-icon>
    <svg-icon icon-class="eye-open"></svg-icon>
    <svg-icon icon-class="eye"></svg-icon>
    <svg-icon icon-class="form"></svg-icon>

  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'name'
    ])
  }
}
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
}
</style>
