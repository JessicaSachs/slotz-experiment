<template>
    <slot>Default BaseButton Text</slot>
</template>

<script>
import { Vue, Component, Prop } from 'vue-property-decorator';

@Component
class BaseButton extends Vue {
}

export default BaseButton;
</script>

<style scoped>

</style>
