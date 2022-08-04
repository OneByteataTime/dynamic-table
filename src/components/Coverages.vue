<template>
    <div class="content">
    <table class="ui table">
        <thead>
            <th class="one wide"></th>
            <th class="six wide">Coverage</th>
            <th class="four wide">Limit</th>
            <th class="four wide">Premium</th>
            <th class="one wide">Override</th>
        </thead>
        <tbody>
            <template v-for="(coverage, index) in coverages">
                <component v-bind:is="coverage.componentName" :key="index" :data="coverage"></component>
            </template>
        </tbody>
    </table>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'
import DriveOtherCar from './DriveOtherCar.vue'
import UnderageDriver from './UnderageDriver.vue'
import Exclusion from './Exclusion.vue'

export default Vue.extend({
    components: {
        DriveOtherCar,
        UnderageDriver,
        Exclusion
    },
    data() {
        return {
            coverages: [
                { id:10, name:"Drive other Car", componentName:"DriveOtherCar" },
                { id:15, name:"Exclusion - Extra data", componentName:"Exclusion"},
                { id:20, name:"Underage Driver", componentName:"UnderageDriver"},
            ]
        }
    }
})
</script>
<style scoped>
    div {
        margin: 1em;
    }
</style>