<template>
    <div>{{num}}</div>
</template>
<script type="text/javascript">
    export default{
        name:'countBox',
        data(){
            return{
                num:0
            }
        },
        methods:{
            addcount(){
                var that = this;
                setInterval(function(){
                    that.num++;
                },1000)
            }
        },
        mounted(){
            this.addcount();
        }
    }
</script>