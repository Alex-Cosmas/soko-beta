<template>
<div class="container">

    <div>

        <div >
            <div>
                <h1 class="text-2xl my-4">Step 1: Registration</h1>
            </div>
            <form>
                <div class="bg-green-200 py-8 px-10 flex flex-col">

                    <div>
                        <div class="flex flex-col my-2">
                            <p class="mt-5">What package will be sending with Sokoplace today?</p>
                            <!-- <legend for="name">Pacakge Details:</legend> -->
                            <input id="name" name="name" placeholder="For Example: Samsung 65 Inch TV" class="py-2 px-3 shadow-xl my-2"></input>
                        </div>

                        <p>Which category best describes your Package</p>

                        <select class="text-primary hover: text-gray-200 px-2 py-1">
                            <option>Select Category</option>
                            <option>Electonics</option>
                            <option>Perishable</option>
                        </select>

                        <p class="mt-5">Anything to note about the package?</p>

                        <div class="flex flex-col my-2">
                            <textarea name="" id="" placeholder="" class="shadow-xl p-4 w-full">

                            </textarea>
                        </div>

                        <div class="flex flex-col my-10">

                            <div class="w-full flex flex-row justify-between">
                                <div class="w-1/2 pr-2">
                                    Senders Details:
                                    <div class="flex flex-col">

                                        <input id="name" name="name" placeholder="Senders Full names" class="py-2 px-3 shadow-xl my-2"></input>

                                        <input id="name" name="package_type" placeholder="Pick Up Location ..." class="py-2 px-3 shadow-xl"></input>

                                        <input id="name" name="package_type" placeholder="Phone Number" class="py-2 px-3 shadow-xl my-2"></input>
                                    </div>
                                </div>
                                <div class="w-1/2 px-2">
                                    Recipient Details:
                                    <div class="flex flex-col">

                                        <input id="name" name="name" placeholder="Recipient Full names" class="py-2 px-3 shadow-xl my-2"></input>

                                        <input id="name" name="package_type" placeholder="Drop Off Location..." class="py-2 px-3 shadow-xl"></input>

                                        <input id="name" name="package_type" placeholder="Phone Number" class="py-2 px-3 shadow-xl my-2"></input>
                                    </div>
                                </div>
                            </div>

                        </div>

                        <button class="bg-primary px-4 py-2 rounded text-white uppercase">Next Step</button>

                    </div>

                </div>
            </form>

        </div>

        <div class="mt-24">
            <div class="">
                <h1 class="text-2xl my-4">Step 2: Confirm & Submit</h1>
            </div>
            <div>
                <form>
                    <div class="bg-green-200 py-8 px-10 flex flex-col">
                        <div>
                            <!-- <div class="flex flex-col my-2">
                                <legend for="name">Pacakge Details:</legend>
                                <input id="name" name="name" placeholder="What package will be sending with Sokoplace today?" class="py-2 px-3 shadow-xl my-2"></input>
                            </div> -->

                            <div>
                                Package Summary
                            </div>

                            <div>
                                Preferred Store

                            </div>
                            <div>
                                <div>
                                    Nearest to Pickup Location: On Toogle Show Select
                                </div>

                            </div>

                            <div class="flex justify-between">
                                 <button class="bg-primary px-4 py-2 rounded text-white uppercase"> < Go Back</button>

                             <nuxt-link to="/client/packages/uploaded" class="bg-primary px-4 py-2 rounded text-white uppercase">+ Add Package</nuxt-link>
                            </div>

                           

                           

                          

                        </div>

                    </div>

                </form>
            </div>
        </div>

    </div>

</div>
</template>

<script>
export default {
    
    // components: {

    // },

    // props: [
    //     'currentStep',
    //     'step1'
    // ], 
    
    // {
    //     title: {
    //         type: String,
    //         required: false,
    //     },
    //     backLink: {
    //         type: String,
    //         required: false,
    //     },
    //     date: {
    //         type: String,
    //         required: false,
    //     }
    // }, 

    // data() {
    //     return {
    //         step:1,
    //         show: true,
    //     };
    // },

    // data: {
    //     currentStep: 1,
    //     package: {
    //         name: '',

    //     }
    // },

    // methods: {
    //     goToStep: function (step) {
    //         this.currentStep = step;
    //     }
    // }

    //   methods: {
    //     display() {
    //       this.show = !this.show;
    //     },
    //   },
}
</script>
