<template>
  <div class="error">
    <p class="error__text">{{ errorMessage }}</p>
  </div>
</template>

<script>
import { mapState } from 'vuex';

export default {
  computed: {
    ...mapState(['errorMessage']),
  },
};
</script>

<style lang="scss" scoped>
.error {
  padding: 0 20px;
  text-align: center;
  &__text {
    margin-top: 10px;
    padding: 5px;
    color: #f00;
    font-size: 14px;
    background-color: #efefef;
  }
}
</style>
