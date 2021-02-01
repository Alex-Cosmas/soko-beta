<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <div>
          
            <h1 class="my-3 text-xl">Store Reports</h1>

           <dataTables/>

          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import NavRoutes from "~/components/NavRoutes/store";
import dataTables from "~/components/dataTables/Store/reports";
export default {
  components: {
    NavRoutes,
    dataTables,
  },
};
</script>

   

