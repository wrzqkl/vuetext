<template>
    <div class="yilaizhuruChild">
        <h3>依赖组件子组件</h3>
        <p>我从父组件收到的财产是：{{ fuqin }}</p>
        <yilaizhuruSun :title="fuqin" :msg="msgggggg"></yilaizhuruSun>
    </div>
</template>
  
<script>
import yilaizhuruSun from '../pages/yilaizhuruSun.vue';
export default {
    name: "yilaizhuruChild",
    data() {
        return {
            msgggggg: 'english'
        }
    },
    components: {
        yilaizhuruSun,
    },
    props: {
        fuqin: {
            type: String,
            default: '10000000',
        }
    }
    // props: ['fuqin']
}
</script>
  
<style scoped>
.yilaizhuruChild {
    color: yellow;
}
</style>