<template>
  <div>
    <ElButton type= "primary" @click="changeA">AboutView</ElButton>
    <el-button type = "warning" @click = "changeA">changeA</el-button>
    <div class="aa">{{ a }}</div>
  </div>
</template>
<script lang="ts">
/**
 * 页面核心数据结构体说明文档
 *
 *
 */
// import from
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'AboutView',
  props: {
    sampleP: {
      type: Number,
      default: 0
    }
  },
  data() {
    return {
      sampleD: 'value',
      a: 3
    }
  },
  computed: {
    /* sampleC() {
      return this.sampleD + "--";
    }, */
  },
  created() {},
  mounted() {},
  methods: {
    // sampleM() {},
    changeA(){
      this.a = this.a+1
    }
  },
  watch: {
    // sampleP(n, o) {},
  }
})
</script>

<!--<style scoped>-->
<style lang="css" scoped>
.aa {
  color: red;
}
</style>