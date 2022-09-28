<template>
    <v-card class="mx-auto pa-md-4 mx-lg-auto" width="400px">
            <v-card-title class="justify-center text-h5 font-weight-bold">
                Gestor de Backup
            </v-card-title>
            <v-card-title class="mx-auto justify-center text-h6 font-weight-bold">
                Inicio de sesion
            </v-card-title>
            <v-text-field v-model="first" label="Usuario" outlined></v-text-field>

            <v-text-field outlined v-model="password" :append-icon="show1 ? 'mdi-eye' : 'mdi-eye-off'"
                :rules="[rules.required]" :type="show1 ? 'text' : 'password'" name="input-10-1" label="Contraseña"
                @click:append="show1 = !show1">
            </v-text-field>

            <v-card-actions class="justify-center">
                <v-btn color="primary" text :to="{path:'/history'}">
                    Iniciar sesión
                </v-btn>
            </v-card-actions>
    </v-card>
</template>

<script>
export default {
    data() {
        return {
            show1: false,
            password: 'Password',
            rules: {
                required: value => !!value || 'Required.',
            }
        }
    },
}
</script>