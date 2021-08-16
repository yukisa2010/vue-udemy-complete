<template>
    <div>
        <slot name="title">Default</slot>
        <slot></slot>
        <slot></slot>
        <slot name="default"></slot>
        <hr/>
        <p>いいねの数</p>
        <slot name="number">Default</slot>
    </div>
</template>

<script>
export default {
    props: ["headerText"]
}
</script>
