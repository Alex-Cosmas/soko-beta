<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <div>
          <!-- <p>Turn Around Time</p> -->

          <dataTables />
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import NavRoutes from "~/components/NavRoutes/analytics";
import dataTables from "~/components/dataTables/Analytics/tat";
export default {
  components: {
    NavRoutes,
    dataTables,
  },
};
</script>

   
