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
    <div class="card-footer text-muted d-flex justify-content-start align-items-center p-3" id="response-container">
        <img src="https://mdbcdn.b-cdn.net/img/Photos/new-templates/bootstrap-chat/ava3-bg.webp" alt="avatar 3"
            style="width: 45px; height: 100%; border-radius: 50%" />
        <input type="text" class="form-control form-control-lg" id="exampleFormControlInput1" placeholder="Type message" />
        <a class="ms-3 text-muted" href="#!"><i class="fas fa-smile"></i></a>
        <a class="ms-3" href="#!"><i class="fas fa-paper-plane"></i></a>
    </div>
</template>

<style scoped>
.form-control {
    border-color: transparent;
}

.form-control:focus {
    border-color: transparent;
    box-shadow: inset 0px 0px 0px 1px transparent;
}
</style>