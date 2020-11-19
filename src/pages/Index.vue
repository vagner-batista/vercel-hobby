<template>
  <q-page class="flex flex-center">
    <div class="full-width row wrap justify-center items-center content-center">
      <div class="col-8  self-center">
        <p>Aqui ficará o canvas para stream da câmera</p>
      </div>
      <div class="q-pa-md col-12">
        <q-carousel
          v-model="slide"
          transition-prev="slide-right"
          transition-next="slide-left"
          swipeable
          animated
          control-color="primary"
          padding
          arrows
          height="300px"
          class="bg-grey-1 shadow-2 rounded-borders blueish"
        >
        <q-carousel-slide :name="1" class="column no-wrap yellowish">
          <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-1.jpeg" />
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-2.jpeg" />
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-3.jpeg" />
          </div>
        </q-carousel-slide>
        <q-carousel-slide :name="2" class="column no-wrap yellowish">
          <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-4.jpeg" />
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-5.jpeg" />
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-6.jpeg" />
          </div>
        </q-carousel-slide>
        <q-carousel-slide :name="3" class="column no-wrap yellowish">
          <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-4.jpeg" />
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-3.jpeg" />
            <q-img class="rounded-borders col-4 full-height redish" src="fotos/foto-5.jpeg" />
          </div>
        </q-carousel-slide>
      </q-carousel>
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
  name: 'PageIndex',
  data () {
    return {
      slide: 1
    }
  }
}
</script>
