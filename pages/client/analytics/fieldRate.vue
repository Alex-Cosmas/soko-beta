<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <div>
          <!-- <p>Field Rate</p> -->

          <dataTables />
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import NavRoutes from "~/components/NavRoutes/analytics";
import dataTables from "~/components/dataTables/Analytics/fieldRate";
export default {
  components: {
    NavRoutes,
    dataTables,
  },
};
</script>

   
