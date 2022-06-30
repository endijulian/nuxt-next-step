<template>
  <div>
      <h1>Test Id {{ $route.params.id }}</h1>
  </div>
</template>

<script>
export default {
    validate({request}){
        return /^\d+$/.test(request.params.id);
    }
}
</script>
