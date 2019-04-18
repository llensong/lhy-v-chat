<template>
    <div class="chatdetails">
        <Daohang/> 
        <div class="content"> 
            <div class="title">评论人名称</div>
            <div class="detaContent">评论内容</div>
                <div >
                    <h5>回复</h5>
                    <div>
                        <Input v-model="value5" type="textarea" placeholder="请输入评论内容" />
                    </div>
                </div>
        </div>
    </div>
</template>
<script>
import Daohang from '@/components/Daohang.vue'//引入路由部分(公用组件)
export default {
    components: {//引入路由部分(公用组件)
            Daohang
    },
    data(){
        return{
            value5:''
        }
    },
    methods:{
        gotoChatContent(){
            this.$router.push({path:'',query:{id:'1'}})
        }
    }
}
</script>