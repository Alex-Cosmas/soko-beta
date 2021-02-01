<template>
  <div>
    <div class="flex mx-auto px-20">
      <div>
        <NavRoutes />

        <div class="w-full flex flex-grow-1">
          <div class="py-6 px-5">
            <div
              class="grid grid-cols-4 grid-flow-row gap-5 flex justify-between min-h-screen"
            >
              <!-- Column 1  -->
              <div class="grid grid-cols-1 gap-2 p-4 h-full">
                <div class="bg-red-200 flex justify-center items-center">
                  <div class="p-3 text-center">
                    <p class="text-5xl">92%</p>
                    <p class="text-sm">Package delivery success rate</p>
                  </div>
                </div>

                <div class="bg-red-200 flex justify-center items-center">
                  <div class="p-3 text-center">
                    <p class="text-5xl">88%</p>
                    <p class="text-sm">On time deliveries</p>
                  </div>
                </div>

                <div class="bg-red-200 flex justify-center items-center">
                  <div class="p-3 text-center">
                    <p class="text-5xl">5%</p>
                    <p class="text-sm">Package returns and damages</p>
                  </div>
                </div>
              </div>

              <!-- Column 2  -->
              <div class="h-screen py-4 flex-grow-1">
                <iframe
                  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d175375.35002233344!2d36.75802242879212!3d-1.2696134355064255!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x182f1172d84d49a7%3A0xf7cf0254b297924c!2sNairobi!5e0!3m2!1sen!2ske!4v1609327678569!5m2!1sen!2ske"
                  width="100%"
                  height="100%"
                  frameborder="0"
                  style="border: 0"
                  allowfullscreen=""
                  aria-hidden="false"
                  tabindex="0"
                ></iframe>
              </div>

              <!-- Column 3  -->
              <div class="grid grid-cols-1 gap-2 p-4 h-full">
                <div class="bg-red-200 py-2 flex flex-col items-center">
                  <p class="font-bold text-center">Todays Highlights</p>
                  <div class="p-3">
                    <p class="text-sm">Dispatched</p>
                    <p class="text-sm">Delivered</p>
                    <p class="text-sm">In-store</p>
                    <p class="text-sm">Returned</p>
                    <p class="text-sm">Uploaded</p>
                  </div>
                </div>

                <div class="bg-red-200 py-2 flex flex-col items-center">
                  <p class="font-bold text-center">
                    In-Store to Dispatch Ratio
                  </p>
                  <div class="p-3"></div>
                </div>
              </div>

              <!-- Column 4  -->
              <div class="grid grid-cols-1 gap-2 p-4 h-full">
                <div class="bg-red-200 py-2 flex flex-col items-center">
                  <p class="font-bold text-center">
                    Number of Packages Delivery
                  </p>
                  <div class="p-3"></div>
                </div>

                <div class="bg-red-200 py-2 flex flex-col items-center">
                  <p class="font-bold text-center">
                    Increase in volume packages
                  </p>
                  <div class="p-3"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavRoutes from "~/components/NavRoutes/analytics";
export default {
  components: {
    NavRoutes,
  },
};
</script>