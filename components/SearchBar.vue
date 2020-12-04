<template>
  <form class="flex flex-1">
    <input
      id="searchbar"
      type="search"
      class="searchBar"
      placeholder="搜尋..."
      @focus="onfocus(true)"
      @blur="onfocus(false)"
      autocomplete="off"
    />
  </form>
</template>
<script>
export default {
  props: ["onfocus"],
};
</script>
<style scoped>
.searchBar {
  @apply border-b flex-1 outline-none p-1 text-gray-600;
}
</style>