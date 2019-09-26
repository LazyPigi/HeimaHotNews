<template>
    <div>
        <HeaderNormal title="我的跟帖"/>

        <!-- 评论的列表 -->
        <div class="comment-item">
            <div class="time">2019-9-25 10:10</div>

            <!-- 当前的评论回复的评论 -->
            <div class="parent">
                <div class="parent-title">
                    @: 瑞强
                </div>
            
                <div class="parent-content">
                    晚饭哪里吃？
                </div>
            </div>
        

            <!-- 个人评论的内容 -->
            <div class="content">
                庆和？
            </div>

            <div class="article-link">
                <router-link to="#">
                    原文：又来到，天亮的泥沼，又想到一起看日出，你用力的抱着我，说怕丢了我，我承诺，一直看到老；爱情像烟灰，不经意灰飞。
                </router-link>
                <span class="iconfont iconjiantou1"></span>
            </div>
        </div>
    </div>
</template>

<script>

// 导入头部
import HeaderNormal from "@/components/HeaderNormal";
export default {
    components: {
        HeaderNormal
    }
}
</script>

<style>

</style>