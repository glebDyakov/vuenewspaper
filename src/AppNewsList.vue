<template>
    <hr>
    <h4>{{ title }}</h4>
    <!-- <ul>
        <li v-for="item in news">
            {{item.title}}
        </li>
    </ul> -->
    <ul>
        <li v-for="item in news" :key="item.id">
            {{item.title}}<span v-if="item.wasRead">!!!</span>
        </li>
    </ul>
</template>
<script>
export default {
    // props:['news'],
    // inject:['title'],
    inject:['title', 'news']
}
</script>