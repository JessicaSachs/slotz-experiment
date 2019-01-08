<template>
    <div class="search-form">
        <div>Hello from the SearchForm.</div>
        <BasePopover
            placement="bottom"
            title="Title"
            width="200"
            trigger="manual"
            content="this is content, this is content, this is content"
        ><slot>Slot from SearchForm</slot></BasePopover>
    </div>
</template>

<script>
import { Vue, Component, Prop } from 'vue-property-decorator';

@Component
class SearchForm extends Vue {
}

export default SearchForm;
</script>

<style scoped>

</style>
