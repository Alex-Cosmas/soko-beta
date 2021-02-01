<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <!-- <div>Package Delivered</div> -->
        <dataTables />
      </div>
    </div>
  </div>
</template>


<script>
import NavRoutes from "~/components/NavRoutes/analytics";
import dataTables from "~/components/dataTables/Analytics/packageDelivery";
export default {
  components: {
    NavRoutes,
    dataTables,
  },
};
</script>

   
