<template>
    <div>
        <iframe :src="address" width="100%" frameborder="0" height="800px"></iframe>
        <el-backtop :visibility-height="60">
            <i class="el-icon-caret-top"></i>
        </el-backtop>
    </div>
</template>

<script>
    export default {
        name: "Quanjing",
        data () {
            return{
                address: "https://venus.sheencity.com/project/publish/d251ff7d-8d4b-4953-a523-af9ad0ddbd90/a8a55f19-8f80-4919-9c36-1118a16820ca/index.html"
            }
        }
    }
</script>

<style scoped>

</style>