<template>
  <div class="mx-auto pa-md-4 mx-lg-auto">
    <h1 class="py-4">
      Gestor de Backup
    </h1>
    <div class="v-flex">
      <v-btn class="mb-4 mx-4" color="primary">Start Backup</v-btn>
      <v-btn class="mb-4 mx-4" color="primary">Stop Backup</v-btn>
    </div>
    <v-card>
      <v-data-table :headers="headers" :items="desserts" fixed-header>
        <template v-slot:item.CBCopiado="{ item }">
          <v-simple-checkbox v-model="item.CBCopiado" disabled></v-simple-checkbox>
        </template>
        <template v-slot:item.CBRestored="{ item }">
          <v-simple-checkbox v-model="item.CBRestored" disabled></v-simple-checkbox>
        </template>
        <template v-slot:item.CBArchivado="{ item }">
          <v-simple-checkbox v-model="item.CBArchivado" disabled></v-simple-checkbox>
        </template>
        <template v-slot:item.CBDepuradoB="{ item }">
          <v-simple-checkbox v-model="item.CBDepuradoB" ></v-simple-checkbox>
        </template>
        <template v-slot:item.CBDepuradoR="{ item }">
          <v-simple-checkbox v-model="item.CBDepuradoR" ></v-simple-checkbox>
        </template>
        <template v-slot:item.CBS="{ item }">
          <v-simple-checkbox v-model="item.CBS" ></v-simple-checkbox>
        </template>
      </v-data-table>

      <v-row align="center" justify="space-around" class=" mx-auto pa-md-5 mx-lg-auto">
        <v-btn color="primary" class="mb-4">
          Hacer Backup
        </v-btn>
        <v-btn color="primary" class="mb-4">
          Copiar a Servidor Restone
        </v-btn>
        <v-btn color="primary" class="mb-4">
          Restaurar en servicios restore
        </v-btn>
        <v-btn color="primary" class="mb-4">
          Empaquetar
        </v-btn>
        <v-btn color="primary" class="mb-4">
          Depurar de servidor backup
        </v-btn>
        <v-btn color="primary" class="mb-4">
          Depurar de servidor restone
        </v-btn>
      </v-row>
    </v-card>
  </div>

</template>

<script>
export default {
  data() {
    return {
      headers: [
        { text: 'backup ID', value: 'numberBID' },
        { text: 'F. Inicio', value: 'dateI' },
        { text: 'F. Final', value: 'dateF' },
        { text: 'Wal Fin', value: 'numberWF' },
        { text: 'Copiado', value: 'CBCopiado' },
        { text: 'restored', value: 'CBRestored' },
        { text: 'Archivado', value: 'CBArchivado' },
        { text: 'Depurado B', value: 'CBDepuradoB' },
        { text: 'Depurado R', value: 'CBDepuradoR' },
        { text: 'S', value: 'CBS' },

      ],
      desserts: [
        {
          numberBID: 987765543,
          dateI: '20/10/11 12:30',
          dateF: '20/10/11 12:30',
          numberWF: 987765524,
          CBCopiado: true,
          CBRestored: true,
          CBArchivado: true,
          CBDepuradoB: true,
          CBDepuradoR: true,
          CBS: true,
        },
        {
          numberBID: 987765543,
          dateI: '20/10/11 12:30',
          dateF: '20/10/11 12:30',
          numberWF: 987765524,
          CBCopiado: true,
          CBRestored: true,
          CBArchivado: true,
          CBDepuradoB: true,
          CBDepuradoR: true,
          CBS: true,
        },
        {
          numberBID: 987765543,
          dateI: '20/10/11 12:30',
          dateF: '20/10/11 12:30',
          numberWF: 987765524,
          CBCopiado: true,
          CBRestored: true,
          CBArchivado: true,
          CBDepuradoB: true,
          CBDepuradoR: true,
          CBS: true,
        },
        {
          numberBID: 987765543,
          dateI: '20/10/11 12:30',
          dateF: '20/10/11 12:30',
          numberWF: 987765524,
          CBCopiado: true,
          CBRestored: true,
          CBArchivado: true,
          CBDepuradoB: true,
          CBDepuradoR: true,
          CBS: true,
        },
        {
          numberBID: 987765543,
          dateI: '20/10/11 12:30',
          dateF: '20/10/11 12:30',
          numberWF: 987765524,
          CBCopiado: true,
          CBRestored: true,
          CBArchivado: true,
          CBDepuradoB: true,
          CBDepuradoR: true,
          CBS: true,
        },
        {
          numberBID: 987765543,
          dateI: '20/10/11 12:30',
          dateF: '20/10/11 12:30',
          numberWF: 987765524,
          CBCopiado: true,
          CBRestored: true,
          CBArchivado: true,
          CBDepuradoB: true,
          CBDepuradoR: true,
          CBS: true,
        },
      ],
    }
  },
}
</script>
