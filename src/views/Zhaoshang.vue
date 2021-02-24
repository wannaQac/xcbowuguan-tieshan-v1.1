<template>
    <div id="content">
        <div class="banner-ld" ng-controller="clgkbanner">
            <img src="../../static/pic18.png" width="100%">
        </div>
        <div class="ui" id="address">
            <div class="mainbox-ld"  ng-controller="clls">
                <div class="title-ld">
                    <div class="title-1">招商引资</div>
                </div>
                <div class="text-ld">
                    <div class="imgvideo">

                    </div>
                </div>
            </div>
        </div>
        <el-backtop :visibility-height="60">
            <i class="el-icon-caret-top"></i>
        </el-backtop>
    </div>
</template>

<script>
    export default {
        name: "Zhaoshang"
    }
</script>

<style scoped>

</style>