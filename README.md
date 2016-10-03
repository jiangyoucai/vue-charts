# vue-charts
charts for vue ,base on echarts

#### how to use

template

    <v-charts
    :x-data="xData"
    :y-data="yData"
    :z-type="zType"></v-charts>

import

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
        created() {},
        methods: {},
        components: {
            'v-charts': Charts
        }
    }

remark

    check the demo or create a issues
