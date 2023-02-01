<template>
  <p class="empty">{{ emptyMessage }}</p>
</template>

<script>
import { mapState } from 'vuex';

export default {
  computed: {
    ...mapState(['emptyMessage']),
  },
};
</script>

<style lang="scss" scoped>
.empty {
  font-size: 14px;
  text-align: center;
}
</style>
