<template>
  <div class="home">
    <h1 class="subtitle-1 grey--text">Dashboard</h1>
    <v-container class="my-5">
      <v-card v-for="project in projects" :key="project.title" class="pa-3" flat>
        <v-row>
          <v-col xs="12" sm="12" md="6">
            <div class="caption">Project Title</div>
            <div>{{project.title}}</div>
          </v-col>
          <v-col xs="5" sm="4" md="2">
            <div class="caption">Person</div>
            <div>{{project.person}}</div>
          </v-col>
          <v-col xs="5" sm="4" md="2">
            <div class="caption">Due by</div>
            <div>{{project.due}}1</div>
          </v-col>
          <v-col xs="2" sm="4" md="2">
            <div class="caption">Status</div>
            <div>{{project.status}}</div>
          </v-col>
        </v-row>
      </v-card>
    </v-container>
  </div>
</template>

<script>
  export default {
    name: 'Dashboard',
    components: {},
    data() {
      return {
        projects: [
          {
            title: 'Design a new website',
            person: 'The Net Ninja',
            due: '1st Jan 2019',
            status: 'ongoing',
            content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt consequuntur eos eligendi illum minima adipisci deleniti, dicta mollitia enim explicabo fugiat quidem ducimus praesentium voluptates porro molestias non sequi animi!'
          },
          {
            title: 'Code up the homepage',
            person: 'Chun Li',
            due: '10th Jan 2019',
            status: 'complete',
            content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt consequuntur eos eligendi illum minima adipisci deleniti, dicta mollitia enim explicabo fugiat quidem ducimus praesentium voluptates porro molestias non sequi animi!'
          },
          {
            title: 'Design video thumbnails',
            person: 'Ryu',
            due: '20th Dec 2018',
            status: 'complete',
            content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt consequuntur eos eligendi illum minima adipisci deleniti, dicta mollitia enim explicabo fugiat quidem ducimus praesentium voluptates porro molestias non sequi animi!'
          },
          {
            title: 'Create a community forum',
            person: 'Gouken',
            due: '20th Oct 2018',
            status: 'overdue',
            content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sunt consequuntur eos eligendi illum minima adipisci deleniti, dicta mollitia enim explicabo fugiat quidem ducimus praesentium voluptates porro molestias non sequi animi!'
          },
        ]
      }
    }
  }
</script>
