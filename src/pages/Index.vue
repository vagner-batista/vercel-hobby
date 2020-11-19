<template>
  <q-page class="flex flex-center">
    <div class="full-width row wrap justify-center items-center content-center">
      <div class="col-8  self-center">
        <p>Aqui ficará o canvas para stream da câmera</p>
      </div>
      <div class="q-pa-md">
        <q-carrousel
          transition-prev="slide-right"
          transition-next="slide-left"
          swipeable
          animated
          control-color="primary"
          navigation
          padding
          arrows
          height="300px"
          class="bg-grey-1 shadow-2 rounded-borders blueish"
        >
        <q-carousel-slide :name="1" class="column no-wrap yellowish">
          <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
            <q-img class="rounded-borders col-6 full-height redish" src="https://cdn.quasar.dev/img/linux-avatar.png" />
            <q-img class="rounded-borders col-6 full-height redish" src="https://cdn.quasar.dev/img/linux-avatar.png" />
            <q-img class="rounded-borders col-6 full-height redish" src="https://cdn.quasar.dev/img/linux-avatar.png" />
            <q-img class="rounded-borders col-6 full-height redish" src="https://cdn.quasar.dev/img/linux-avatar.png" />
          </div>
        </q-carousel-slide>
      </q-carrousel>
      </div>
    </div>
  </q-page>
</template>

<style lang='scss' scoped>
.redish{
  background-color:$red-5;
}
.blueish{
  background-color:$blue-4;
}
.yellowish{
  background-color:$amber-13;
}
</style>

<script>
export default {
  name: 'PageIndex'
}
</script>
