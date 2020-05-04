<template>
  <div>
    <h1>A single user view vith ID: {{ $route.params.id }}</h1>
  </div>
</template>
 
 <script>
export default {
  validate(data) {
    //console.log(data);
    return /^\d+$/.test(data.params.id);
  }
};
</script>