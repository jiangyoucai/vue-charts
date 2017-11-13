# vue-charts

a charts component base on echarts
#### install
npm

    npm install tt-vue-charts

yarn

    yarn add tt-vue-charts

#### how to use

template

    <v-charts
    :x-data="xData"
    :y-data="yData"
    :z-type="zType"></v-charts>

import

    import Charts from 'tt-vue-charts'
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
