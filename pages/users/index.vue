<template>
  <div>
    <h1>The Users view</h1>
    <input type="text" v-model="userId" />
    <button @click="onLoadUser">Load user</button>
  </div>
</template>
<script>
export default {
  data() {
    return {
      userId: ""
    };
  },
  methods: {
    onLoadUser() {
      this.$router.push(`/users/${this.userId}`);
    }
  }
};
</script>