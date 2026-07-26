<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 137****1100 策划了神级签到系统玄幻前三章大纲"
  },
  {
    "text": "用户 189****4422 生成了末世囤货流打脸吸血亲戚的爆点线路"
  },
  {
    "text": "用户 131****8899 完成了女频穿书大佬手撕绿茶白莲花剧本"
  },
  {
    "text": "用户 156****3310 生成了万倍返还神豪流打脸拜金女全套 SOP"
  },
  {
    "text": "用户 173****5588 取得了 100 万字玄幻换地图升级路线"
  }
]);
</script>
