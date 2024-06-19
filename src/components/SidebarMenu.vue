<script setup>
import { useRoute } from 'vue-router';
const router = useRoute()
import Cookies from 'js-cookie';
const logout = () => {
    Cookies.remove('token')
    Cookies.remove('user')
    router.push({name:'login'})
}
</script>

<template>
    <div class="card bourder-0 rounded shadow-sm">
        <div class="card-header">MENU UTAMA</div>
    </div>
    <div class="card-body">
        <div class="list-group">
            <router-link :to="{name: 'dashboard'}" class="list-group-item list-group-item-action">DASHBOARD</router-link>
            <router-link :to="{name: 'admin.users.index'}" class="list-group-item list-group-item-action">USER</router-link>
            <a href="#" @click="logout" class="list-group-item list-group-item-action">Logout</a>
        </div>
    </div>
</template>