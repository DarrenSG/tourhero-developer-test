<script setup>
import ItineraryIcon from '@/components/icons/ItineraryIcon.vue'
import ItineraryItem from '@/components/ItineraryItem.vue'
</script>

<template>
  <section>
    <div class="flex items-end gap-2 mb-6">
      <ItineraryIcon class="w-7" />
      <div class="text-blue-900 font-bold text-xl leading-none">Itinerary</div>
    </div>

    <div class="flex flex-col gap-10 mb-6">
      <ItineraryItem
        day="1"
        title="See the largest indoor water fall in the world"
        excerpt="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur aut, dolor harum magnam maxime obcaecati quas repellendus rerum sapiente totam vel voluptate voluptatum!"
      >
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
      </ItineraryItem>

      <ItineraryItem
        day="2"
        title="Two giant conversations"
        excerpt="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur aut, dolor harum magnam maxime obcaecati quas repellendus rerum sapiente totam vel voluptate voluptatum!"
      >
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
      </ItineraryItem>

      <ItineraryItem
        day="3"
        title="Singapore's 21st-century botanical garden"
        excerpt="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur aut, dolor harum magnam maxime obcaecati quas repellendus rerum sapiente totam vel voluptate voluptatum!"
      >
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
      </ItineraryItem>

      <ItineraryItem
        day="4"
        title="Super Park"
        excerpt="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur aut, dolor harum magnam maxime obcaecati quas repellendus rerum sapiente totam vel voluptate voluptatum!"
      >
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consectetur consequatur enim
          iusto odit omnis praesentium quaerat soluta tenetur. Accusantium debitis deserunt ducimus
          ea laborum, magnam omnis quae sapiente tempore totam?
        </p>
      </ItineraryItem>
    </div>
  </section>
</template>
