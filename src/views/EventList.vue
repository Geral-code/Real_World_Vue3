<template>
<h1>Events for Good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event"/>

   
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from '@/components/EventCard.vue'

export default {
  name: 'EventList',
  components: {
    EventCard
  },

   data() {
        return {
            events: [
            {
                id: 5928101,
                category: 'animal welfare',
                title: 'Cat Adoption Day',
                description: 'Find your new feline friend',
                location: 'Miau Town',
                date: 'Jan 1st, 2022',
                time: '12:00',
                petsAllowed: true,
                organizer: 'Kat Laydee'
            },
            {
                id: 4582797,
                category: 'food',
                title: 'Community Garding',
                description: 'Join us',
                location: 'Plant Town',
                date: 'Jan 2nd, 2022',
                time: '12:00',
                petsAllowed: true,
                organizer: 'Fern Poline'

            },
            {
                id: 2547697,
                category: 'sustainability',
                title: 'Beach Cleanup',
                description: 'Help us cleaning up',
                location: 'Playa El Tabo',
                date: 'Jan 3rd, 2022',
                time: '12:00',
                petsAllowed: false,
                organizer: 'Carey Wales'
            }
            
            ]

        }
    }
}
</script>
<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
