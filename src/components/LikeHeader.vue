<template>
    <div>
        <slot :user="user" text="text"></slot>
        <slot></slot>
        <hr>ß
        <p>いいねの数</p>
        <slot></slot>
    </div>
</template>

<script>
export default {
    data() {
        return {
            user: {
                firstName: 'Jack',
                lastName: 'Donald'
            }
        }
    }
}
</script>
