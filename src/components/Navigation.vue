<template>
    <div>
        <mu-appbar style="width: 100%;" color="primary" z-depth="1">
            <mu-button icon slot="left" @click="isOpenDrawer=!isOpenDrawer">
                <mu-icon value="menu"></mu-icon>
            </mu-button>
            Jusic 点歌台
        </mu-appbar>
        <mu-drawer width="300" :open.sync="isOpenDrawer" :docked="false" :right="false">
            <mu-card style="width: 100%; max-width: 375px; margin: 0 auto;">
                <mu-card-header title="H" sub-title="Shanghai, China">
                    <mu-avatar size="45" slot="avatar">
                        <img style="border-radius: 50%; border: 1px solid rgba(255, 255, 255, 0.2);" src="../assets/images/uicon.jpg">
                    </mu-avatar>
                </mu-card-header>
                <mu-card-media title="Jusic" sub-title="Just music"
                               style="max-height: 200px; overflow: hidden">
                    <img src="../assets/images/fl.jpg">
                </mu-card-media>
                <mu-card-text>
                    聊天、斗图、音乐、点播、娱乐
                </mu-card-text>
            </mu-card>
            <mu-list>
                <mu-sub-header>社交</mu-sub-header>
                <mu-list-item button href="https://github.com/hanhuoer" target="_blank">
                    <mu-list-item-title>Github</mu-list-item-title>
                </mu-list-item>
                <mu-list-item button href="mailto:hanhuoer@126.com" target="_blank">
                    <mu-list-item-title>邮箱</mu-list-item-title>
                </mu-list-item>
                <mu-divider></mu-divider>
                <mu-sub-header>关于</mu-sub-header>
                <mu-list-item button href="https://github.com/hanhuoer/Jusic-ui" target="_blank">
                    <mu-list-item-title>Jusic-ui</mu-list-item-title>
                </mu-list-item>
                <mu-list-item button href="https://github.com/hanhuoer/Jusic-serve" target="_blank">
                    <mu-list-item-title>Jusic-serve</mu-list-item-title>
                </mu-list-item>
                <mu-sub-header>反馈</mu-sub-header>
                <mu-tooltip content="Jusic 点歌台反馈：985590542">
                    <mu-list-item button href="https://jq.qq.com/?_wv=1027&k=5MBUzwC" target="_blank">
                        <mu-list-item-title>QQ Group</mu-list-item-title>
                    </mu-list-item>
                </mu-tooltip>
            </mu-list>
        </mu-drawer>
    </div>
</template>

<script>
    export default {
        name: "Navigation",
        data: () => ({
            isOpenDrawer: false
        })
    }
</script>

<style scoped>

</style>
