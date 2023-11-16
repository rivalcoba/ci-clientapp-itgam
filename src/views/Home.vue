<script setup>
import { storeToRefs } from 'pinia';

import { useAuthStore } from '@/stores';

const authStore = useAuthStore();
const { user } = storeToRefs(authStore);
</script>

<template>
    <div v-if="user">
        <h1>Hola {{user.firstName}}!</h1>
        <p>Has iniciado sesión en el Sistema de Administración de la Biblioteca del ITGAM</p>
        <center><img srcset="src/views/users/biblio.jpg" width="600" height="500"/></center>
        <br><br>
    </div>
    <body>
        <form>
                        <center>  <div class="media-container-row mbr-white" style="font-family:Roboto,'Opens Sans', sans-serif">
                                <div class="col-12 col-md-3 mbr-fonts-style display-7" style="font-family:Roboto,'Opens Sans', sans-serif" >
                                    <p class="mbr-text" style="color:darkblue">
                                        <strong>Dirección:</strong>
                                        <br>
                                        <br><a style="color:black">Calle 608 No. 300 y Av. 412, Col. San Juan de Aragón, Alcaldía. Gustavo A. Madero, C.P. 07470, México, CDMX</a><br>
                                        <br>
                                        <br><strong>Contacto:</strong>&nbsp;<br>
                                        <br><a style="color:black">Teléfonos: <br>
                                            (55) 2651-7864 y (55) 2651-6275 </a><br></p>
                                </div>
                                </div>
                                <div class="col-12 col-md-3 mbr-fonts-style display-7" style="font-family:Roboto,'Opens Sans', sans-serif">
                                    <p class="mbr-text" style="color:darkblue"><strong>Redes Sociales</strong><br>
                                        <br>
                                        <a style="color:red" href="https://web.facebook.com/profile.php?id=100032494910892">Facebook</a><br>
                                        <a style="color:red" href="https://www.instagram.com/tecnm_itgam/">Instagram</a><br>
                                        <a style="color:red" href="https://www.gamadero.tecnm.mx/" data-toggle="modal" data-target="#modalQuejas">Página Oficial</a><br>
                                        
                                        <br>
                                        <strong>Localizacion en el Mapa: </strong>
                                        <img srcset="src/views/users/mapa.png" width="707" height="500"/>
                                    </p>
                                </div></center>
                                <center><div class="media-container-row mbr-white" style="font-family:Roboto,'Opens Sans', sans-serif">
                                    <div class="col-sm-6 copyright">
                                        <p class="mbr-text mbr-fonts-style display-7"> Copyright © 2023 Eduardo Guerrero Rodríguez</p>
                                        <br />
                                <strong>SISTEMA DE ADMINISTRACION DE LA BIBLIOTECA DEL ITGAM</strong>
                                        <p class="mbr-text mbr-fonts-style display-7">Última actualización: 02/10/2023</p>
                                    </div>
                                </div></center>
                            </form>
    </body>
</template>