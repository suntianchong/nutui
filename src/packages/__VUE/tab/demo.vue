<template>
  <div class="demo full">
    <h2>基础用法</h2>
    <nut-tab>
      <nut-tab-panel tab-title="全部"
        ><p class="content">这里是页签全部内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待付款"
        ><p class="content">这里是页签待付款内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待收获"
        ><p class="content">这里是页签待收获内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="已完成"
        ><p class="content">这里是页签已完成内容</p></nut-tab-panel
      >
    </nut-tab>

    <h2>defaultIndex设置默认显示tab</h2>
    <h2>switchTab监听切换tab返回事件</h2>
    <nut-tab :default-index="1" @switch-tab="switchTab">
      <nut-tab-panel tab-title="全部"
        ><p class="content">这里是页签全部内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待付款"
        ><p class="content">这里是页签待付款内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待收获"
        ><p class="content">这里是页签待收获内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="已完成"
        ><p class="content">这里是页签已完成内容</p></nut-tab-panel
      >
    </nut-tab>

    <h2> animatedTime 开启切换标签内容时的转场动画时间</h2>
    <nut-tab :animated-time="500">
      <nut-tab-panel tab-title="全部"
        ><p class="content">这里是页签全部内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待付款"
        ><p class="content">这里是页签待付款内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待收获"
        ><p class="content">这里是页签待收获内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="已完成"
        ><p class="content">这里是页签已完成内容</p></nut-tab-panel
      >
    </nut-tab>

    <h2> 禁止tab内容滑动</h2>
    <nut-tab :no-swiping="true">
      <nut-tab-panel tab-title="全部"
        ><p class="content">这里是页签全部内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待付款"
        ><p class="content">这里是页签待付款内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待收获"
        ><p class="content">这里是页签待收获内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="已完成"
        ><p class="content">这里是页签已完成内容</p></nut-tab-panel
      >
    </nut-tab>

    <h2
      >标签数量超过 5
      个时，标签栏可以在水平方向上滚动，切换时会自动将当前标签居中。</h2
    >
    <nut-tab :animated-time="500">
      <nut-tab-panel tab-title="全部"
        ><p class="content">这里是页签全部内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待付款"
        ><p class="content">这里是页签待付款内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待收获"
        ><p class="content">这里是页签待收获内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="已完成"
        ><p class="content">这里是页签已完成内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="已取消"
        ><p class="content">这里是页签已取消内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待评价"
        ><p class="content">这里是页签待评价内容</p></nut-tab-panel
      >
    </nut-tab>

    <h2>设置slot:header可以自定义标签</h2>
    <nut-tab>
      <nut-tab-panel tab-title="全部">
        <template v-slot:header><nut-icon name="dongdong"></nut-icon></template>
        <p class="content">这里是页签全部内容</p>
      </nut-tab-panel>
      <nut-tab-panel tab-title="待付款"
        ><p class="content">这里是页签待付款内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待收获"
        ><p class="content">这里是页签待收获内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="已完成"
        ><p class="content">这里是页签已完成内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="已取消"
        ><p class="content">这里是页签已取消内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="待评价"
        ><p class="content">这里是页签待评价内容</p></nut-tab-panel
      >
    </nut-tab>

    <h2>左右tab布局</h2>
    <nut-tab direction="vertical" :animated-time="500" :default-index="2">
      <nut-tab-panel tab-title="页签一"
        ><p class="content">这里是页签一内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="页签二"
        ><p class="content">这里是页签二内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="页签三"
        ><p class="content">这里是页签三内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="页签四"
        ><p class="content">这里是页签四内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="页签五"
        ><p class="content">这里是页签五内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="页签六"
        ><p class="content">这里是页签六内容</p></nut-tab-panel
      >
      <nut-tab-panel tab-title="页签七"
        ><p class="content">这里是页签七内容</p></nut-tab-panel
      >
    </nut-tab>

    <h2>异步操作</h2>
    <nut-tab :animated-time="500" v-if="editList.length > 0">
      <nut-tab-panel
        :tab-title="item.title"
        v-for="(item, index) in editList"
        :key="index"
      >
        <p class="content">这里是页签{{ index }}内容</p>
      </nut-tab-panel>
    </nut-tab>
    <nut-button type="primary" @click="changeList">改变数据</nut-button>
  </div>
</template>

<script lang="ts">
import { ref, reactive, toRefs } from 'vue';
import { createComponent } from '@/packages/utils/create';
const { createDemo } = createComponent('tab');
export default createDemo({
  props: {},
  setup() {
    const resData = reactive({
      editList: [
        {
          title: '标签一'
        },
        {
          title: '标签二'
        }
      ]
    });
    function changeList() {
      resData.editList.push({
        title: '标签' + resData.editList.length
      });
    }
    function switchTab(activeInddex: number, event: MouseEvent) {
      console.log(activeInddex, event);
    }
    return {
      ...toRefs(resData),
      changeList,
      switchTab
    };
  }
});
</script>

<style lang="scss" scoped>
.content {
  padding: 10px;
}
</style>
