<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <h1 class="my-3 text-xl">Dispatched Packages</h1>
        <dataTables />
      </div>
    </div>
  </div>
</template>


<script>
import NavRoutes from "~/components/NavRoutes/packages";
import dataTables from "~/components/dataTables/Packages/dispatched";
export default {
  components: {
    NavRoutes,
    dataTables,
  },
};
</script>

   
