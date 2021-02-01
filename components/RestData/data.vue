<template>
  <section class="info container mx-auto px-10 my-10">
    <div v-for="store in fooddata" :key="store.id" class="">
      <h1 class="text-3xl">{{ store.name }}</h1>
      <div>
        <div class="flex justify-between">
          <p>Delivery Time: {{ store.deliveryTime }}</p>
          <p>Store Rating: {{ store.rating }}</p>
          <p v-if="store.freeDelivery" class="label">
            <span>Free Delivery</span>
          </p>
        </div>
      </div>

      <div class="row flex flex-row mt-3 mb-8 w-full ">
        <div
          v-for="menuitem in store.menu"
          :key="menuitem.id"
          class="items w-full flex justify-between"
        >
          <div class="info bg-gray-600 w-full mx-2 p-10">
            <div>
              <h4 class="text-xl">{{ menuitem.item }}</h4>
              <h4>{{ menuitem.price }}</h4>
              <button class="bg-primary px-4 py-1 rounded-md">View Item</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { mapState } from "vuex";

export default {
  computed: {
    ...mapState(["fooddata"])
  }
};
</script>
