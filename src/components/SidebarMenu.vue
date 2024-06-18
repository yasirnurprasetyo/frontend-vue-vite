<script setup>
</script>

<template>
    <div class="card bourder-0 rounded shadow-sm">
        <div class="card-header">MENU UTAMA</div>
    </div>
    <div class="card-body">
        <div class="list-group">
            <router-link :to="{name: 'dashboard'}" class="list-group-item list-group-item-action">DASHBOARD</router-link>
            <a href="#" class="list-group-item list-group-item-action">Users</a>
            <a href="#" class="list-group-item list-group-item-action">Logout</a>
        </div>
    </div>
</template>