<script setup>
import '@splidejs/vue-splide/css'
import { Splide } from '@splidejs/vue-splide'
import VideoSlide from '@/components/VideoSlide.vue'
import ItineraryList from '@/components/ItineraryList.vue'
import StarRating from '@/components/StarRating.vue'
import HeartIcon from '@/components/icons/HeartIcon.vue'
import AppButton from '@/components/AppButton.vue'
import QuickInfo from '@/components/QuickInfo.vue'
import ItineraryHeader from '@/components/ItineraryHeader.vue'
</script>

<template>
  <Splide
    :options="{
      rewind: true,
      fixedWidth: '1120px',
      gap: '1rem',
      focus: 'center',
      start: 1,
      trimSpace: false,
      pagination: false
    }"
  >
    <VideoSlide src="https://picsum.photos/id/50/1120/400" />
    <VideoSlide src="https://picsum.photos/id/10/1120/400" />
    <VideoSlide src="https://picsum.photos/id/20/1120/400" />
  </Splide>

  <main
    class="max-w-6xl mx-auto border-blue-500 mt-8 lg:mt-0 lg:-translate-y-10 grid lg:grid-cols-3 gap-4 px-3 lg:px-1"
  >
    <section class="bg-white lg:col-span-2 rounded-lg lg:shadow px-4 lg:px-8 py-6">
      <ItineraryHeader />
      <ItineraryList class="hidden lg:block" />
    </section>

    <section>
      <div
        class="bg-blue-900 rounded-t-lg px-6 py-6 text-white flex-col items-center gap-1 hidden lg:flex"
      >
        <div class="text-sm text-gray-300 uppercase">From</div>
        <div class="text-3xl font-medium">1,300 USD</div>
        <div class="text-sm text-gray-300">
          <span class="line-through">1,699 USD</span> PER PERSON
        </div>
        <div class="flex items-center gap-1 my-1 mb-4">
          <StarRating :stars="4" class="mr-2" />
          <small>4.8</small>
          <small class="text-gray-400">(23)</small>
        </div>
        <div class="flex w-full gap-2">
          <AppButton class="flex-1 bg-red-600">Book Trip</AppButton>
          <AppButton class="px-2.5">
            <HeartIcon class="w-4" />
          </AppButton>
          <AppButton class="px-3">Share</AppButton>
        </div>
      </div>

      <div class="lg:border-t-0 lg:border p-4 lg:p-6 grid grid-cols-3 gap-y-6 gap-x-3 rounded-b-lg">
        <QuickInfo icon="schedule" label="Duration" text="3 Days" />
        <QuickInfo icon="language" label="Countries" text="2" />
        <QuickInfo icon="sprint" label="Activity Level" text="Streneous" />
        <QuickInfo icon="translate" label="Guide Language" text="English" />
        <QuickInfo
          icon="checklist"
          label="inclusion"
          text="Food, Hotel, Transport"
          class="col-span-2"
        />
      </div>
      <div class="my-5 border text-center py-8 rounded-lg">
        <span class="material-symbols-outlined text-gray-400 text-[100px]">map</span>
      </div>
      <div class="my-5 lg:border p-4 lg:p-6 rounded-lg flex flex-col">
        <div class="flex items-center gap-2 mb-5">
          <span class="material-symbols-outlined text-cyan-700">shopping_cart</span>
          <span class="text-blue-900 font-bold text-lg leading-none">Buy With Confidence</span>
        </div>
        <div class="flex items-center gap-1.5">
          <span class="material-symbols-outlined text-cyan-700 text-lg pt-0.5">check_circle</span>
          <span class="text-sm font-medium">0% Installment Payment</span>
        </div>
        <div class="flex items-center gap-1.5">
          <span class="material-symbols-outlined text-cyan-700 text-lg pt-0.5">check_circle</span>
          <span class="text-sm font-medium">$200 Deposit</span>
        </div>
        <div class="flex items-center gap-1.5">
          <span class="material-symbols-outlined text-cyan-700 text-lg pt-0.5">check_circle</span>
          <span class="text-sm font-medium">24/7 Support</span>
        </div>
        <div class="flex items-center gap-1.5">
          <span class="material-symbols-outlined text-cyan-700 text-lg pt-0.5">check_circle</span>
          <span class="text-sm font-medium">No Booking Fee</span>
        </div>
        <div class="flex items-center gap-1.5">
          <span class="material-symbols-outlined text-cyan-700 text-lg pt-0.5">check_circle</span>
          <span class="text-sm font-medium">Free Cancellations</span>
        </div>
      </div>
    </section>

    <ItineraryList class="block lg:hidden px-4" />
  </main>
</template>

<style scoped></style>
