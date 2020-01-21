<template>
    <div>
        <PetsTable species="cats" :pets="cats" />
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
    ...mapState([
      'cats'
    ])
  }
}
</script>
