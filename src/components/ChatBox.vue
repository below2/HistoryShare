<script setup>
import ChatMessageReceived from './ChatMessageReceived.vue'
import ChatMessageSent from './ChatMessageSent.vue'
import ChatFooter from './ChatFooter.vue'
// imports
// defineProps({
//   msg: {
//     type: String,
//     required: true
//   }
// })
</script>

<template>
    <section class="section d-flex align-items-center py-5">
        <div class="container" style="height: 100%">
            <div style="height: 100%">
                <div class="card" id="chat2" style="height: 100%">
                    <div class="card-header d-flex justify-content-between align-items-center p-3">
                        <h5 class="mb-0">History</h5>
                    </div>
                    <div class="card-body overflow-auto" style="position: relative; height: 400px">
                        <ChatMessageReceived>
                            <template #chat-message-received>Test</template>
                            <template #chat-message-received-time>12:34</template>
                        </ChatMessageReceived>
                        <ChatMessageSent>
                            <template #chat-message-sent>Test1</template>
                            <template #chat-message-sent-time>00:00</template>
                        </ChatMessageSent>

                        <div class="divider d-flex align-items-center mb-4">
                            <p class="text-center mx-3 mb-0" style="color: #a2aab7">
                                Today
                            </p>
                        </div>
                    </div>
                    <ChatFooter />
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.section {
    height: 100%;
    margin: 0;
    background-color: #eee;
}

.divider:after,
.divider:before {
    content: "";
    flex: 1;
    height: 1px;
    background: #eee;
}
</style>