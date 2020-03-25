<template>
  <div class="equityPage">
    <equityList />
  </div>
</template>

<script>
// @ is an alias to /src
import equityList from "@/components/equityList.vue";

export default {
  name: "package",
  components: {
    equityList
  }
};
</script>
