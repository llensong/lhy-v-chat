<template>
    <div class="details">
        <Daohang/> 
        <div class="content"> 
            <div class="title">标题名称</div>
            <div class="detaContent">标题内容</div>
            <div class="detailChat">
                <div class="chatDetails">
                    评论区,显示已评论内容
                    <ul>
                        <li>
                            <div>评论内容</div>
                            <div>
                                <h5 @click="gotoChatContent()">查看</h5>
                            </div>
                            <div >
                                <h5>回复</h5>
                                <div>
                                    <Input v-model="value5" type="textarea" placeholder="请输入评论内容" />
                                    <button type="submit">发送</button>
                                </div>
                            </div>
                        </li>
                    </ul>
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
            this.$router.push({path:'chatdetails',query:{id:'1'}})
        }
    }
}
</script>