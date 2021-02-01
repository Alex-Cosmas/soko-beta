<template>
  <div>
    <form method="post">
      <div v-show="step === 1">
        <h1>Step 1</h1>

        <div>
          <input type="text" v-model="registration.name" placeholder="name" />
        </div>
        <div>
          <input type="text" v-model="step1.email" placeholder="email" />
        </div>

        <button type="button" @click.prevent="next()">Next</button>
      </div>
    </form>
    <!-- <div id="step2" v-if="currentStep == 2">
      <h1>Step 2</h1>

      <div>
        <input
          type="text"
          name="city"
          v-model="step2.city"
          placeholder="city"
        />
      </div>
      <div>
        <input
          type="text"
          name="state"
          v-model="step2.state"
          placeholder="state"
        />
      </div>

      <button type="button" @click.prevent="goToStep(3)">Finish</button>
    </div>
    <div id="step3" v-if="currentStep == 3">
      <strong>Name:</strong> {{ step1.name }}<br />
      <strong>Email:</strong> {{ step1.email }}<br />
      <strong>City:</strong> {{ step2.city }}<br />
      <strong>State:</strong> {{ step2.state }}
    </div>
   -->
  </div>
</template>

<script>
export default {
  data: {
    step: 1,
    registration: {
      name: "null"
    }
  },
  methods: {
    prev() {
      this.step--;
    },
    next() {
      this.step++;
    }
  }
};
</script>
