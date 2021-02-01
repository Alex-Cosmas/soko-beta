<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col">
        <NavRoutes />
        <div>
          
            <h1 class="my-3 text-xl">Add Stores - Modal</h1>
            <div>
              
              <!--  -->
              <p>Code</p>
              <p>Name</p>
              <p>User</p>
              <p>Location</p>
              <p>Industry</p>
              <p>License</p>
              <p>Phone</p>
              <p>Select Fleet</p>
            </div>

           

          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import NavRoutes from "~/components/NavRoutes/store";

export default {
  components: {
    NavRoutes,
  },
};
</script>

   

