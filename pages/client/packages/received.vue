  
<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <div>
          
            <h1 class="my-3 text-xl">Received Packages</h1>

            <dataTables />

          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import NavRoutes from "~/components/NavRoutes/packages";
import dataTables from "~/components/dataTables/Packages/received";
export default {
  components: {
    NavRoutes,
    dataTables,
  },
};
</script>

   

