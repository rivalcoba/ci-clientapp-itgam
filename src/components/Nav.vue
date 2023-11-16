<script setup>
import { useAuthStore } from '@/stores';


const authStore = useAuthStore();
</script>

<template>
    <body>
    <header><img srcset="src/views/itgambanner.jpg" width="807" height="111" style="position: initial; top: 0; right: 0;" /></header>

    </body>
    <nav v-show="authStore.user" class="navbar navbar-expand navbar-blue bg-dark">
        <div class="navbar-nav">
            <router-link to="/" class="nav-item nav-link">Inicio</router-link>
            <router-link to="/users" class="nav-item nav-link">Administrar Usuarios</router-link>
            <router-link to="" class="nav-item nav-link">Inventario de libros</router-link>
            <router-link to="" class="nav-item nav-link">Revisión Cuentas Especiales</router-link>
            <router-link to="" class="btn btn-link">Registro Diario</router-link>
            <!--<router-link to="" class="nav-item nav-link">Registro de Libro</router-link>
            <router-link to="" class="nav-item nav-link">Prestamos</router-link>
            <router-link to="" class="nav-item nav-link">Solicitudes de Renovación</router-link>-->
            <button @click="authStore.logout()" class="btn btn-link nav-item nav-link">Cerrar Sesión</button>
        </div>
    </nav>
</template>