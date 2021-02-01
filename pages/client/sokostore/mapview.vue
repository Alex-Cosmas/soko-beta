<template>
  <div>
    <div class="flex mx-auto px-20">
      <div class="flex flex-col w-full">
        <NavRoutes />
        <div>
          
            <h1 class="my-3 text-xl">Map View</h1>

            <div class="">      

                <div class="">
                  <input class="px-4 py1" placeholder="Enter your location" />

                  <iframe
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d175375.35002233344!2d36.75802242879212!3d-1.2696134355064255!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x182f1172d84d49a7%3A0xf7cf0254b297924c!2sNairobi!5e0!3m2!1sen!2ske!4v1609327678569!5m2!1sen!2ske"
                    width="100%"
                    height="100%"
                    frameborder="0"
                    style="border: 0"
                    allowfullscreen=""
                    aria-hidden="false"
                    tabindex="0"
                    class="min-h-full min-w-full"
                  ></iframe>
                </div>
              
            </div>
            

           

          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import NavRoutes from "~/components/NavRoutes/store";
import dataTables from "~/components/dataTables/Store/mapview";

export default {
  components: {
    NavRoutes,
    dataTables,
  },
};
</script>

   

