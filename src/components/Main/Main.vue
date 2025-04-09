<template>
    <main>
        <Performance></Performance>
        <Result></Result>
        <Item></Item>
        <Company></Company>
        <Sketchbook></Sketchbook>
    </main>
</template>

<script>
import Performance from './Performance/Performance.vue';
import Result from './Result/Result.vue';
import Item from './Item/Item.vue';
import Company from './Company/Company.vue';
import Sketchbook from './Sketchbook/Sketchbook.vue';
export default {
    name: "Main",
    components: { Performance, Result, Item, Company, Sketchbook }
}
</script>