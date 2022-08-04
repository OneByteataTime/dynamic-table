<template>
    <tr>
        <td><div class="ui input"><input type="checkbox" name="" id=""></div></td>
        <td>{{data.name}}</td>
        <td><div class="ui mini input"><input class="ui input" type="text" name="" id=""></div></td>
        <td><div class="ui mini input"><input class="ui input" type="text" name="" id="" value="$100.00"></div></td>
    </tr>
</template>
<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    name: 'DriveOtherCar',
    props: {
        data: Object
    }
})
</script>