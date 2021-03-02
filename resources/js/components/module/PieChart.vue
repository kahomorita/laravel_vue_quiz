<script>
    import{Pie} from "vue-chartjs";
    export default {
        extend: Pie,
        props:{
            chartData:{
                type:Object
            }
        },
        methods:{
            renderPieChart() {
                this.renderChart(this.chartData,{
                    borderWidth:"10px",
                    hoverBackgroundColor: "red",
                    hoverBorderWidth: "10px"
                });
            }
        }
    };
</script>
