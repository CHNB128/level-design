<template>
  <div 
    class="modal fade" 
    id="modal" 
    tabindex="-1" 
    role="dialog" 
    aria-labelledby="exampleModalLabel" 
    aria-hidden="true">
    <div 
      class="modal-dialog" 
      role="document">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title">Modal title</h5>
          <button type="button" class="close" data-dismiss="modal" aria-label="Close">
            <span aria-hidden="true">&times;</span>
          </button>
        </div>
        <div class="modal-body">
          <load-level v-if="$store.state.modal.type = 'load-level'"/>
          <!--          <load-level v-if="$store.state.modal.type = 'save-level'"/> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LoadLevel from './LoadLevel'

export default {
  components: {
    LoadLevel
  }
}
</script>
