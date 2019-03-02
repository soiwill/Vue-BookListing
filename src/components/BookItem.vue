<template>
    <li>{{book.title}}:{{book.author}}</book
</template>

<script>
export default {
    title: "BookItem",
    props: ["book"]
}
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>
