<template>
    <el-popover v-bind="$attrs" v-model="visible">
        <slot slot="reference" @click="visible = !visible">Slot from BasePopover</slot>
    </el-popover>
</template>

<script>
import { Vue, Component, Prop } from 'vue-property-decorator';
import { Popover } from 'element-ui';

@Component({ components: { 'el-popover': Popover }})
class BasePopover extends Vue {
}

export default BasePopover;
</script>

<style scoped>

</style>
