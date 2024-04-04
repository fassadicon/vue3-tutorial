<script>
// script setup
// import HelloWorld from "./components/HelloWorld.vue";
// import TheWelcome from "./components/TheWelcome.vue";
import Home from "./views/Home.vue";
import Home2 from "./components/Home2.vue";

// export default {
//   name: "App",
//   data() {
//     return {
//       formValues: {
//         name: "",
//         profile: "",
//         country: "",
//         jobLocation: [],
//         remoteWork: "no",
//         skillSet: [],
//         yearsOfExperience: '',
//         age: null
//       }
//     }
//   },
//   methods: {
//     submitForm () {
//       console.log(this.formValues)
//     }
//   }
// };
</script>

<template>
  <Home></Home>
  <Home2></Home2>
  <Home/>
  <Home2/>
  <!-- <pre>
    {{ formValues }}
  </pre> -->
  <!-- <form @submit.prevent="submitForm">
    <div>
      <label for="name">Name</label>
      <input type="text" id="name" v-model.trim.lazy="formValues.name">
    </div>
    <div>
      <label for="age">Age</label>
      <input @keyup.enter="submitForm" type="number" id="age" v-model.number="formValues.age">
    </div>
    <div>
      <label for="profile">Profle</label>
      <textarea type="text" id="profile" v-model="formValues.profile" />
    </div>
    <div>
      <label for="country">Country</label>
      <select id="country" v-model="formValues.country">
        <option value="">Select a country</option>
        <option value="philippines">Philippines</option>
        <option value="singapore">Singapore</option>
        <option value="canada">Canada</option>
      </select>
    </div>
    <div>
      <label for="jobLocation">Job Location</label>
      <select id="jobLocation" multiple v-model="formValues.jobLocation">
        <option value="philippines">Philippines</option>
        <option value="singapore">Singapore</option>
        <option value="canada">Canada</option>
      </select>
    </div>
    <div>
      <input type="checkbox" id="remoteWork" v-model="formValues.remoteWork" true-value="yes" false-value="no">
      <label for="remoteWork">Open to remote work?</label>
    </div>
    <div id="skillSets">
      <label for="skillSets">Skill Sets</label>
      <input type="checkbox" id="HTML" value="html" v-model="formValues.skillSet">
      <label for="HTML">HTML</label>
      <input type="checkbox" id="CSS" value="css" v-model="formValues.skillSet">
      <label for="CSS">CSS</label>
      <input type="checkbox" id="JS" value="js" v-model="formValues.skillSet">
      <label for="JS">JS</label>
    </div>
    <div id="yearsOfExperience">
      <label for="yearsOfExperience">Years of Experience</label>
      <input type="radio" id="0-2" value="0-2" v-model="formValues.yearsOfExperience">
      <label for="0-2">0 - 2</label>
      <input type="radio" id="3-5" value="3-5" v-model="formValues.yearsOfExperience">
      <label for="3-5">3 - 5</label>
      <input type="radio" id="6-8" value="6-8" v-model="formValues.yearsOfExperience">
      <label for="6-8">6 - 8</label>

    </div>
  </form> -->
</template>

<!-- <style scoped>
.underlined {
  text-decoration: underline;
}

.lined-through {
  text-decoration: line-through;
}

.yellow {
  color: yellow;
}

/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style> -->
./components/Topbar.vue