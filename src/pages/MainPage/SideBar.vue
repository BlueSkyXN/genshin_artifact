<template>
    <div class="root">
        <el-menu
            default-active="intro"
            style="border: none"
            router
        >
            <el-menu-item index="intro">
                <i class="el-icon-s-home"></i>
                <span>首页</span>
            </el-menu-item>

            <el-menu-item-group>
                <template #title>
                    圣遗物
                </template>
                <el-menu-item index="artifacts">
                    <i class="el-icon-s-help"></i>
                    添加圣遗物
                </el-menu-item>
            </el-menu-item-group>

            <el-menu-item-group>
                <template #title>
                    计算
                </template>
                <el-menu-item index="calculate">
                    <i class="el-icon-cpu"></i>
                    Arts Planner
                </el-menu-item>
            </el-menu-item-group>

            <!-- <el-menu-item-group>
                <template #title>
                    帮助
                </template>
                <el-menu-item index="use-case">
                    <i class="el-icon-question"></i>
                    完整使用示例
                </el-menu-item>
                <el-menu-item index="alg">
                    <i class="el-icon-s-opportunity"></i>
                    算法
                </el-menu-item>
            </el-menu-item-group> -->
        </el-menu>
    </div>
</template>

<script>
export default {
    name: "SideBar",
    props: {
        items: {
            type: Array,
            default: () => [],
        }
    }
}
</script>

<style scoped>
.top {
    height: 220px;
    background: #409eff;
    display: flex;
    align-items: center;
    justify-content: center;
}

/* .root {
    background: #123456;
} */

.item {
    padding: 0 32px;
}
</style>