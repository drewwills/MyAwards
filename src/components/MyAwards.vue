<template>
  <div class="awards">
    <h2>{{ msg }}</h2>
    <ul v-if="awards && awards.length">
      <li v-for="(award, index) in awards" :key="index">
        <div>{{ award.id }} {{ award.title }}</div>
      </li>
    </ul>

    <ul v-if="errors && errors.length">
      <li v-for="(error, index) in errors" :key="index">{{ error.message }}</li>
    </ul>
  </div>
</template>

<script>
import Vue from 'vue';

export default {
  name: 'MyAwards',
  data() {
    return {
      msg: 'My Active Awards',
      awards: [
        {
          id: '00-0000',
          sponsor: 'Baylor College of Medicine',
          title: 'Training in Precision Environmental Health Sciences',
          startDate: '01-JAN-2019',
          endDate: '01-FEB-2023',
          Amount: '150,000',
        },
        {
          id: '00-0001',
          sponsor: 'Defense Agency',
          title: 'Predicting antibiotic resistance: Moving from reaction ....',
          startDate: '01-MAR-2016',
          endDate: '01-FEB-2019',
          Amount: '1,000,000',
        },
        {
          id: '00-0002',
          sponsor: 'National Institutes of Health (NIH)',
          title: 'Defining Evolutionary Trajectories...',
          startDate: '01-JAN-2014',
          endDate: '01-MAR-2019',
          Amount: '500,000',
        },
        {
          id: '00-0003',
          sponsor: 'The TAMU System Health Science Ctr',
          title: 'IBT Cell....',
          startDate: '01-JAN-2016',
          endDate: '01-JAN-2020',
          Amount: '100,000',
        },
        {
          id: '00-0004',
          sponsor: 'University of Texas Health Science Center-Houston',
          title: 'Antimicrobial peptide...',
          startDate: '01-DEC-2018',
          endDate: '01-FEB-2023',
          Amount: '150,000',
        },
      ],
      errors: [],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.awards {
  max-width: 600px;
  margin: auto;
}
li {
  border: none;
  width: 600px;
  text-align: left;
}
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
