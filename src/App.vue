<script setup lang="ts">
import { reactive} from "vue";
import zhCn from 'element-plus/lib/locale/lang/zh-cn'

const state = reactive<any>({
  locale: zhCn
});
</script>

<template>
  <el-config-provider :locale="state.locale">
    <div class="container" style="width: 1200px; margin: 0 auto;padding-top:20px">
      <XmwPer/>
    </div>
  </el-config-provider>
</template>
