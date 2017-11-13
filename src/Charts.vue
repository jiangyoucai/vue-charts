<template lang="html">
    <div class="charts" id="charts">
    </div>
</template>

<script>
import Echarts from 'Echarts'
export default {
    props: ['xData', 'yData', 'zType'],
    data() {
        return {}
    },
    watch: {
        xData() {
            this.createCharts()
        },
        yData() {
            this.createCharts()
        },
        zType() {
            this.createCharts()
        }
    },
    computed: {},
    created() {
        this.createCharts()
    },
    methods: {
        createCharts() {
            const container = document.getElementById('charts')
            const charts = Echarts.init(container)
            charts.setOption({
                title: {},
                tooltip: {},
                xAxis: {
                    data: this.xData
                },
                yAxis: {},
                series: [{
                    type: this.zType,
                    data: this.yData
                }]
            })
        }
    },
    components: {}
}
</script>

<style lang="css">
    .charts{
        clear: both;
        width: 100%;
        min-height: 60vh;
    }
</style>
