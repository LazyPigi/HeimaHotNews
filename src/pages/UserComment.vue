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

            <router-link to="#" class="article-link">
                <p>
                原文：又来到，天亮的泥沼，又想到一起看日出，你用力的抱着我，说怕丢了我，我承诺，一直看到老；爱情像烟灰，不经意灰飞。
                </p>
                <span class="iconfont iconjiantou1"></span>
            </router-link>
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

<style scoped lang="less">
.comment-item {
    padding: 10px;
    font-size: 14px;
    line-height: 1.8;
    border-bottom: 1px #ccc solid;

    .time {
        font-size: 12px;
        color: #999;
        margin-bottom: 5px;
    }

    .parent {
        background: #eee;
        padding: 10px;
        margin-bottom: 5px;

        .parent-title {
            font-size: 12px;
            color: #999;
        }
    }

    .content {
        margin-bottom: 5px;
    }

    .article-link {
        display: flex;
        justify-content: space-between;
        align-items: center;
        font-size: 12px;
        color: #999;

        p {
            overflow: hidden;
            text-overflow: ellipsis;
            white-space: nowrap;
        }
    }
}
</style>