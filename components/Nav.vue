<template>
  <div class="nav">
    <Logo v-if="!isSearching" />
    <SearchBar :onfocus="focusChanged" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      isSearching: false,
    };
  },
  methods: {
    focusChanged(bool) {
        this.isSearching = bool;
    },
  },
};
</script>

<style scoped>
.nav {
  @apply flex justify-start p-3;
}
</style>