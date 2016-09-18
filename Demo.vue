<template lang="html">
    <v-charts :x-data="xData" :y-data="yData" :z-type="zType"></v-charts>
</template>

<script>
import Charts from './Charts'
export default {
    data() {
        return {
            xData: ['js', 'python', 'php', 'lua', 'golang', 'java'],
            yData: ['100', '85', '63', '71', '92', '78'],
            zType: 'line'
        }
    },
    computed: {},
    ready() {},
    attached() {},
    methods: {},
    components: {
        'v-charts': Charts
    }
}
</script>

<style lang="css">
</style>
