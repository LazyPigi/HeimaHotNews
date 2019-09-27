<template>
    <div class="card">
        <!-- 左侧文字 -->
        <div class="card-left">
            <div class="post-title">
                回忆与我都不爱说话,偶尔我会想起他,心里有一些牵挂,有些爱却不得不各安天涯...
                回忆与我都不爱说话,偶尔我会想起他,心里有一些牵挂,有些爱却不得不各安天涯...
                回忆与我都不爱说话,偶尔我会想起他,心里有一些牵挂,有些爱却不得不各安天涯...
            </div>
            <p class="post-info">
                <span>网易云音乐</span>
                <span>100跟帖</span>
            </p>
        </div>

        <div class="card-img">
            <img src="https://ss2.bdstatic.com/70cFvnSh_Q1YnxGkpoWK1HF6hhy/it/u=3815925718,1170141200&fm=26&gp=0.jpg" alt="">
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="less">
    .card{
        padding: 20px 10px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        border-bottom: 1px #ccc solid;

        .card-left{
            flex:1;

            .post-title{
                font-size: 14px;
                line-height: 1.5;
                margin-bottom: 5px;
                display: -webkit-box;
                -webkit-box-orient: vertical;
                -webkit-line-clamp: 2;
                overflow: hidden;
            }

            .post-info{
                font-size:12px;
                color:#999;
            }
        }

        .card-img{
            img{
                display: block;
                width: 120 / 360 * 100vw;
                height: 80 / 360 * 100vw;
                object-fit: cover;
            }
        }
    }
</style>