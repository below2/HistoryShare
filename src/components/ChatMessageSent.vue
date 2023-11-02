<script setup>
// imports
// defineProps({
//   msg: {
//     type: String,
//     required: true
//   }
// })
</script>

<template>
    <div class="d-flex flex-row justify-content-end mb-4 pt-1">
        <div style="padding-right: 10px;">
            <p class="small p-2 me-3 mb-1 text-white rounded-lg bg-primary">
                <slot name="chat-message-sent"></slot>
            </p>
            <p class="small me-3 mb-3 rounded-3 text-muted d-flex justify-content-end">
                <slot name="chat-message-sent-time"></slot>
            </p>
        </div>
        <img src="https://mdbcdn.b-cdn.net/img/Photos/new-templates/bootstrap-chat/ava3-bg.webp" alt="avatar 1"
            style="width: 45px; height: 100%; border-radius: 50%" />
    </div>
</template>

<style scoped>
/* styling */
</style>