<template>
    <!--section 1 navbar-->
    <nav class=" bg-gray-800">
        <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
            <div class="relative flex h-16 items-center justify-between">
                <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
                    <!-- Mobile menu button-->
                    <button type="button"
                        class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
                        aria-controls="mobile-menu" aria-expanded="false">
                        <span class="absolute -inset-0.5"></span>
                        <span class="sr-only">Open main menu</span>

                        <svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                            aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                        </svg>

                        <svg class="hidden h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                            aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                    </button>
                </div>
                <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">

                    <div class="hidden sm:ml-6 sm:block">
                        <div class="flex space-x-4">
                            <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
                            <a href="#" class="bg-gray-900 text-white rounded-md px-3 py-2 text-sm font-medium"
                                aria-current="page">Dashboard</a>
                            <a href="#"
                                class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Master
                                Price</a>
                            <a href="#"
                                class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Custom
                                Price</a>

                            <a href="#"
                                class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Calender</a>
                            <a href="#"
                                class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Reports</a>

                        </div>
                    </div>
                </div>
                <div class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0">
                    <button type="button"
                        class="relative rounded-full bg-gray-800 p-1 text-gray-400 hover:text-white focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800">
                        <span class="absolute -inset-1.5"></span>
                        <span class="sr-only">View notifications</span>
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                            aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round"
                                d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0" />
                        </svg>
                    </button>
                    <!--profile dropdown-->
                    <div class="relative ml-3">
                        <div>
                            <button type="button"
                                class="relative flex rounded-full bg-gray-800 text-sm focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800"
                                id="user-menu-button" aria-expanded="false" aria-haspopup="true">
                                <span class="absolute -inset-1.5"></span>
                                <span class="sr-only">Open user menu</span>
                                <img class="h-8 w-8 rounded-full" src="./assets/Ishrat.jpg" alt="">
                            </button>
                        </div>




                    </div>
                </div>
            </div>
        </div>

        <!-- Mobile menu, show/hide based on menu state. -->
        <div class="sm:hidden" id="mobile-menu">
            <div class="space-y-1 px-2 pb-3 pt-2">
                <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
                <a href="#" class="bg-gray-900 text-white block rounded-md px-3 py-2 text-base font-medium"
                    aria-current="page">Dashboard</a>
                <a href="#"
                    class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Master
                    Price</a>
                <a href="#"
                    class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Custom
                    Price</a>
                <a href="#"
                    class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Calender</a>
                <a href="#"
                    class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Reports</a>

            </div>
        </div>
    </nav>
    <!--section 2-->
    <div class="border-solid border-b-2 border-gray-300 mb-2">
        <h3 class=" font-bold text-3xl ml-32">Master Price</h3>
    </div>

    <!--section 3-->
    <div class="w-10/12 ml-40 my-4">
        <div class="flex justify-center items-center pb-4  border-b-2 border-indigo-300">
            <div class="grid grid-cols-3 ">
                <div class="font-bold text-xs col-span-1 bg-gray-200 px-4 py-2 border border-gray-400"><a href="#">Round
                        Trip</a></div>
                <div class="font-bold text-xs col-span-1 text-white bg-indigo-900 px-4 py-2 border border-gray-400"><a
                        href="#">One Way</a>
                </div>
                <div class="font-bold text-xs col-span-1 bg-gray-200 px-4 py-2 border border-gray-400"><a href="#">Multi
                        City</a></div>
            </div>
        </div>
        <!--input section-->
        <div class="border-b-2 border-indigo-300">
            <div class="forms ">
                <form class="w-full mx-auto">
                    <div class="flex flex-wrap">

                        <div class="ml-2 my-2">
                            <input
                                class="appearance-none block w-36 px-4 py-2 leading-tight font-semibold bg-white border border-black text-gray-700 text-sm   dark:border-gray-600 dark:placeholder-gray-400 dark:text-white "
                                type="text" placeholder="LHR" />
                        </div>
                        <div class="ml-2 my-2">
                            <input
                                class="appearance-none block w-36 px-4 py-2 leading-tight  font-semibold bg-blue-100 border border-black text-stone-700 text-sm dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-800 dark:text-white "
                                type="text" placeholder="CDG" />
                        </div>


                        <div>





                            <div class="antialiased sans-serif">
                                <div x-data="app()" x-init="[initDate(), getNoOfDays()]" x-cloak>
                                    <div class="container  px-2   mt-2">
                                        <div class=" w-44  bg-blue-100">


                                            <div class="relative text-xs  ">
                                                <input type="hidden" name="date" x-ref="date">
                                                <input type="text" readonly x-model="datepickerValue"
                                                    class="w-full h-9  bg-blue-100 pl-4 pr-10 py-2 leading-none border border-black shadow-sm focus:outline-none focus:shadow-outline text-gray-600 font-medium"
                                                    placeholder="22-12-2022">

                                                <div class="absolute  top-0 right-0 px-3 pt-2">
                                                    <svg class="h-5 w-5 text-gray-400" fill="none" viewBox="0 0 24 24"
                                                        stroke="currentColor">
                                                        <path stroke-linecap="round" stroke-linejoin="round"
                                                            stroke-width="2"
                                                            d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                                                    </svg>
                                                </div>






                                            </div>
                                        </div>

                                    </div>
                                </div>


                            </div>

                        </div>
                        <div>


                        </div>
                        <div class="ml-2 my-2">
                            <div class="relative">
                                <select
                                    class="appearance-none block w-20 px-3 py-2 pr-8 font-semibold bg-white border border-black text-gray-700 text-sm   dark:border-gray-600 dark:placeholder-gray-400 dark:text-white">
                                    <option value="">Day-</option>
                                </select>
                                <div
                                    class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 font-bold text-gray-500">
                                    <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg"
                                        viewBox="0 0 20 20">
                                        <path
                                            d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="ml-2 my-2">
                            <div class="relative">
                                <select
                                    class="appearance-none block w-20 px-3 py-2 pr-8 font-semibold bg-white border border-black text-gray-700 text-sm   dark:border-gray-600 dark:placeholder-gray-400 dark:text-white">
                                    <option value="">Day+</option>
                                </select>
                                <div
                                    class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 font-bold text-gray-500">
                                    <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg"
                                        viewBox="0 0 20 20">
                                        <path
                                            d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="ml-2 my-2">
                            <div class="relative">
                                <select
                                    class="appearance-none block w-56 px-3 py-2  font-semibold bg-white border border-black text-gray-700 text-sm   dark:border-gray-600 dark:placeholder-gray-400 dark:text-white">
                                    <option value="">Any Time</option>
                                </select>
                                <div
                                    class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 font-bold text-gray-500">
                                    <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg"
                                        viewBox="0 0 20 20">
                                        <path
                                            d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="font-semibold text-2xl ml-2 mt-2">+</div>
                        <div class="ml-2 my-2">
                            <div class="relative">
                                <select
                                    class="appearance-none  block w-36 px-3 py-2 font-semibold bg-white border border-black text-gray-700 text-sm   dark:border-gray-600 dark:placeholder-gray-400 dark:text-white">
                                    <option value="">ADT</option>
                                </select>
                                <div
                                    class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 font-bold text-gray-500">
                                    <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg"
                                        viewBox="0 0 20 20">
                                        <path
                                            d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="ml-2 my-2">
                            <div class="relative">
                                <select
                                    class="block appearance-none w-36  border border-black font-bold text-gray-500 py-2 px-4   leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
                                    id="grid-state">
                                    <option value="">1</option>
                                </select>
                                <div
                                    class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 font-bold text-gray-500">
                                    <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg"
                                        viewBox="0 0 20 20">
                                        <path
                                            d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z" />
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div class="font-semibold text-2xl ml-4  mt-2 ">+</div>

                    </div>
                </form>
            </div>

        </div>
        <div class="extra mt-4 border-b-2 border-blue-500">
            <div class="flex flex-row">
                <div>
                    <div class="block form-check">
                        <input
                            class="form-check-input appearance-none h-4 w-4 border border-gray-600 rounded-sm bg-white checked:bg-blue-600 checked:border-blue-600 focus:outline-none transition duration-200 mt-1 align-top bg-no-repeat bg-center bg-contain float-left mr-2 cursor-pointer"
                            type="checkbox" id="flexCheckDefault">
                    </div>
                </div>
                <div class="environment  flex-row">

                    <div class=" ">

                        <label class="ml-2    font-bold text-black dark:text-gray-300">Extra
                            Options</label>
                    </div>
                </div>
                <div class="environment flex-row">

                    <div class=" ">

                        <label class="ml-80 labelEnv font-bold text-black dark:text-gray-300">Environment</label>
                    </div>
                </div>
                <div class="environment flex-row">

                    <div class=" ">
                        <input checked id="default-radio-2" type="radio" value="" name="default-radio"
                            class="mt-1 ml-4 file:w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600">

                    </div>
                </div>
                <div class="environment flex-row">

                    <div class=" ">

                        <label class="ml-2 mt-1  font-bold text-black dark:text-gray-300">Dummy</label>
                    </div>
                </div>
                <div class="environment flex-row">

                    <div class=" ">
                        <input checked id="default-radio-2" type="radio" value="" name="default-radio"
                            class="mt-1 ml-2 file:w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600">

                    </div>
                </div>
                <div class="environment flex-row">

                    <div class=" ">

                        <label class="ml-2 mt-1 mr-96  font-bold text-black dark:text-gray-300">PDT</label>
                    </div>
                </div>
                <div class="button flex-row">
                    <button
                        class="bg-indigo-900 ml-76 hover:bg-blue-900 text-white  py-1 px-4 mb-1 border border-blue-700 rounded">
                        SEARCH
                    </button>
                </div>
            </div>
        </div>


        <!--table-->
        <div class="relative overflow-x-auto shadow-md sm:rounded-lg">
            <h4 class="font-bold mb-2">Data Parsed Successfully</h4>
            <table class="w-full text-sm text-left rtl:text-right text-gray-500 dark:text-gray-400">
                <thead class="text-xs py-1 text-gray-600 uppercase bg-gray-300 dark:bg-gray-700 dark:text-gray-400">
                    <tr>
                        <th scope="col" class="px-6 py-3">
                            FLIGHT
                        </th>
                        <th scope="col" class="px-6 py-3">
                            AIRCRAFT
                        </th>
                        <th scope="col" class="px-6 py-3">
                            CLASS
                        </th>
                        <th scope="col" class="px-6 py-3">
                            FARE
                        </th>
                        <th scope="col" class="px-6 py-3">
                            ROUTE
                        </th>
                        <th scope="col" class="px-6 py-3">
                            DEPARTURE
                        </th>
                        <th scope="col" class="px-6 py-3">
                            ARRIVAL
                        </th>
                        <th scope="col" class="px-6 py-3">
                            DURATION
                        </th>
                        <th scope="col" class="px-6 py-3">
                            PRICE
                        </th>
                    </tr>
                </thead>
                <tbody>
                    <tr v-for="flight in flightOffer.flightOffer"
                        class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
                        <td class="px-6 py-3">

                            <div v-for="itineraris in flight.itineraries">
                                <div v-for="segments in itineraris.segments">
                                    {{ segments.marketingCarrier }} {{ segments.aircraft }}
                                </div>

                            </div>
                        </td>
                        <td class="px-6 py-3">
                            <div v-for="itineraris in flight.itineraries">
                                <div v-for="segments in itineraris.segments">
                                    {{ segments.flightNumber }}
                                </div>

                            </div>
                        </td>
                        <td class="px-6 py-3">
                            <div v-for="flightClass in flight.class">
                                <div v-for="flClass in flightClass">
                                    {{ flClass }}
                                </div>

                            </div>
                        </td>
                        <td class="px-6 py-3">
                            <div v-for="fareBasis in flight.fareBasis">
                                <div v-for="fare in fareBasis">
                                    {{ fare }}
                                </div>

                            </div>
                        </td>
                        <td class="px-6 py-3">
                            <div v-for="itineraris in flight.itineraries">
                                <div v-for="segments in itineraris.segments">
                                    {{ segments.departure.iataCode }} - {{ segments.arrival.iataCode }}
                                </div>

                            </div>
                        </td>
                        <td class="px-6 py-3">
                            <div v-for="itineraris in flight.itineraries">
                                <div v-for="segments in itineraris.segments">
                                    {{ segments.departure.at }}
                                </div>

                            </div>
                        </td>
                        <td class="px-6 py-3">
                            <div v-for="itineraris in flight.itineraries">
                                <div v-for="segments in itineraris.segments">
                                    {{ segments.arrival.at }}
                                </div>

                            </div>
                        </td>
                        <td class="px-6 py-3">
                            <div v-for="itineraris in flight.itineraries">
                                {{ itineraris.duration }}

                            </div>
                        </td>

                        <td class="px-6 py-3">
                            <div class="flex flex-col">

                                <div>{{ flight.price }}</div>
                                <div>
                                    <button
                                        class="bg-indigo-900 ml-76 hover:bg-blue-900 text-white  py-1 px-4 mb-1 border border-blue-700 rounded">
                                        SEARCH
                                    </button>
                                </div>
                            </div>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>
<script>
import jsonData from '../public/data.json';
export default {
    data() {
        return {
            flightOffer: jsonData
        };
    }
};
</script>