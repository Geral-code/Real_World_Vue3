<template>
   <div class="event-card"> 
  <span>@ {{ event.time }} on {{ event.date }} </span>
  <h4>{{ event.title }} </h4>
  </div> 
</template>

<script>
export default {
    data(){
        return {
            event: null
        }
    },
    created (){
        // fetch event (by id) and set local data

    }

}
</script>

<style>

</style>