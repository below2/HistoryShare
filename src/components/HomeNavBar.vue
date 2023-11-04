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
    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg fixed-top bg-light navbar-light">
        <div class="container" style="width: 100%; max-width: 100%;">
            <a class="navbar-brand" href="#">
                <div style="display: flex;">
                    <h1 class="text-primary" id="logo">History</h1>
                    <h1 class="text-muted">Share</h1>
                </div>
            </a>
            <button class="navbar-toggler" type="button" data-mdb-toggle="collapse"
                data-mdb-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                aria-label="Toggle navigation">
                <i class="fas fa-bars"></i>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent" style="justify-content: right;">
                <ul class="navbar-nav ms-auto align-items-center">
                    <li class="nav-item">
                        <a class="nav-link mx-2" href="#!"><i class="fas fa-plus-circle pe-2"></i> Invite</a>
                    </li>
                    <li class="nav-item ms-3">
                        <a class="btn btn-dark btn-rounded" href="#!">Sign in</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <!-- Navbar -->
</template>
  
<style scoped>
.navbar-light .navbar-nav .nav-link {
    color: #000;
}
</style>
  