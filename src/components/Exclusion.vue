<template>
    <fragment>
        <tr>
            <td><input type="checkbox" name="" id=""></td>
            <td>{{data.name}}</td>
            <td><div class="ui mini input"><input type="text" name="" id="" /></div></td>
            <td><div class="ui mini input"><input type="text" name="" id="" value="$1,000.00" /></div></td>
            <td><div class="ui mini input"><input type="checkbox" name="" id="" /></div></td>
        </tr>
        <tr class="multi-row">
            <td class="extra"></td>
            <td class="extra" colspan="3">
                <div class="ui mini input">
                    <input type="text" class="wide" name="" id="" placeholder="Description" />
                </div>
            </td>
            <td class="extra"></td>
        </tr>
        <tr>
            <td class="extra"></td>
            <td class="extra" colspan="3">
                <div class="ui mini input">
                    <input type="text" class="wide" name="" id="" placeholder="Locations">
                </div>
            </td>
            <td class="extra"></td>
        </tr>
    </fragment>
</template>
<script lang="ts">
import Vue from 'vue'
import { Fragment } from 'vue-fragment'

export default Vue.extend({
    name: 'UnderageDriver',
    components: {
        Fragment
    },
    props: {
        data: Object
    }
})
</script>
<style scoped>
    td.extra {
        border: none !important;
    }

    input[type="text"].wide {
        width: 600px;
        display: inline-block;
        margin-left: 1em;
    }
</style>