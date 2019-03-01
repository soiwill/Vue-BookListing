<template>
<div>
    <h1>{{title}}</h1>
    <ul>
        <li>Book 1</li>
        <li>Book 2</li>
        <li>Book 3</li>
    </ul>
    <ul>
        <li v-for="book in books">{{book.title}}... Content:{{book.author}}</li>
    </ul>
    
</div>

</template>

<script>
export default {
    name: "BookList",
    data(){
        return {
            title: "All Books",
            books: [
                {title:"Sol", author:"Sol Author"},
                {title:"Yvonne", author:"Yvonne Author"},
                {title:"Daughter", author:"Daughter"}
            ]
        }
    }
}
</script>

<style>
h1, h2 {
    font-weight: normal
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: block;
    padding: 0 10px;
}
</style>
