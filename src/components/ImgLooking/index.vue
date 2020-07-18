<!-- 图片放大查看组件 -->
<template>
    <div>
        <img class="small-img" :src="url" @click="previewImg" />
        <el-dialog title="提示" :visible.sync="centerDialogVisible" width="35%">
            <img class="large-img" :src="url" />
        </el-dialog>
    </div>
</template>

<script>
    export default {
        props: {
            url: {
                type: String,
                default: '',
            }
        },
        data() {
            return {
                //url: 'https://fuss10.elemecdn.com/e/5d/4a731a90594a4af544c0c25941171jpeg.jpeg',
                centerDialogVisible: false,
            }
        },
        //生命周期 - 创建完成（访问当前this实例）
        created() {},
        //生命周期 - 挂载完成（访问DOM元素）
        mounted() {},
        methods: {
            previewImg() {
                this.centerDialogVisible = true;
            }
        }
    }
</script>

<style scoped>
    /* @import url(); 引入css类 */
    .small-img {
        width: 50px;
        height: 50px;
    }
    .large-img {
        width: 400px;
        height: 400px;
    }
</style>