<template>
    <!-- @input是输入框每次输入时候都会触发 -->
    <!-- :class值如果是对象的话，key是class的名称，如果这个key的值是true时候就加上该class -->
    <input 
    class="input" 
    :class="{
        success: status === 'success',
        error: status === 'error'
    }"
    :placeholder="placeholder" 
    :value="value" 
    @input="handleInput" 
    @change="handleChange"
    />
</template>

<script>
export default {
    data(){
        return {
            status: ""
        }
    },
    // rule传递过来的正则表达式
    props: [
        "placeholder",
        "value",
        "name",

        "rule",
        "err_message"
    ],

    // mounted(){
    //     console.log(this.rule)
    // },

    methods: {
        // 每次输入框值时都会触发
        handleInput(event){
            // this.$emit("input", event.target.value)
            const {value} = event.target;

            // 触发父组件的input事件，返回输入框的值
            this.$emit("input", value);

            // 如果符合正则就位success，反之是error
            if(this.rule){
                if( this.rule.test(value) ){
                    this.status = "success";
                }else {
                    this.status = "error";
                }
            }
        },

        // 输入框失去焦点时触发
        handleChange(){
            if(this.err_message && this.status === "error"){
                // alert(this.err_message);
                this.$toast.fail(this.err_message)
            }
        }
    }
};
</script>

<style scoped lang="less">
.input{
    width: 100%;
    height: 38 / 360 * 100vw;
    padding: 20px 0;
    box-sizing: border-box;
    background: #fff;
    border: none;
    border-bottom: 1px #666 solid;
    outline: none;
    font-size: 18px;
}

.success {
    border-bottom-color: blue;
}

.error {
    border-bottom-color: red;
}
</style>