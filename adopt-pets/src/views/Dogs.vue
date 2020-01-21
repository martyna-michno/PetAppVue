
<template>
    <div>
        <PetsTable species="dogs" :pets="dogs" />
    </div>
</template>
<script>
import { mapState } from 'vuex'
import PetsTable from '@/components/PetsTable'

export default {
  components: {
    PetsTable
  },
  data () {
    return {}
  },
  computed: {
    ...mapState(['dogs'])
  }
}
</script>
