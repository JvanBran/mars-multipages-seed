<template>
  <div class="container">
    <div class="btn-group">
      <button class="btn btn-primary" @click="showLoading">
        showLoading
      </button>
      <button class="btn btn-primary" @click="hideLoading">
        hideLoading
      </button>
      <button class="btn btn-primary" @click="goIndex">
        Back
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Loading',
  data() {
    return {}
  },
  computed: {
  },
  mounted() {
  },
  created() {
  },
  methods: {
    showLoading: function() {
      this.$loading.show();
    },
    hideLoading: function() {
      this.$loading.hide();
    },
    goIndex: function() {
      this.$router.push('/');
    }
  }
}
</script>
<style lang="scss" scoped>
@import "~@/assets/sass/base/mixins";
@import "~@/assets/sass/base/weui_button";

.container {
    display: flex;
    width: 100%;
    padding: 20px;
}

</style>
