<template>
    <tr>
        <td><input type="checkbox" name="" id=""></td>
        <td>{{data.name}}</td>
        <td><div class="ui mini input"><input type="text" name="" id=""></div></td>
        <td><div class="ui mini input"><input type="text" name="" id="" value="$400.50"></div></td>
        <td><input type="checkbox" name="" id=""></td>
    </tr>
</template>
<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'UnderageDriver',
    props: {
        data: Object
    }
})
</script>