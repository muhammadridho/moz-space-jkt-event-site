<template>
<div>
 <v-layout row wrap justify-center align-center>
   <v-flex xs12>
      <h2 class="text-xs-center">Selamat datang Keyholder</h2>
   </v-flex>
 </v-layout>
  <v-layout row wrap align-center justify-center>
    <v-flex xs12 
            sm6 
            md6>
      <event-table title="Acara Mendatang"/>
    </v-flex>
    <v-flex xs12 sm6 md6>
      <event-table title="Event belum terkonfirmasi" :confirmed="false"></event-table>
    </v-flex>
  </v-layout>
</div>
</template>
<script>
import EventTable from '@/components/Events/EventTable'

export default {
  components: {
    EventTable,
  } 
}
</script>
