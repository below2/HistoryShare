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
    <div class="d-flex flex-row justify-content-start">
        <img src="https://mdbcdn.b-cdn.net/img/Photos/new-templates/bootstrap-chat/ava4-bg.webp" alt="avatar 1"
            style="width: 45px; height: 100%; border-radius: 50%" />
        <div style="padding-left: 10px;">
            <div style="display: flex; align-items: flex-end">
                <p class="small p-2 ms-3 mb-1 rounded-lg" style="background-color: #f5f6f7">
                    <slot name="chat-message-received"></slot>
                </p>
                <i class="bi bi-reply-fill" id="button-reply" style="align-self: flex-end; height: 20px; width: 20px"></i>
            </div>
            <p class="small ms-3 mb-3 rounded-3 text-muted">
                <slot name="chat-message-received-time"></slot>
            </p>
        </div>
    </div>
</template>

<style scoped>
/* styling */
</style>