<template lang="">
    <div
    class="entry-container mb-3 pointer p-2"
    @click="$router.push({name:'entry',params:{id:10}})">
    <!-- titulo -->
      <div class="entry-title d-flex">
          <span class="text-success fs-5 fw-bold">15</span>
          <span class="mx-1 fs-5">julio</span>
          <span class="mx-2 fw-light">2023, jueves</span>
  
      </div>
      <div class="entry-description">
            Elit sint consectetur ex culpa cupidatat esse culpa irure. Nostrud consequat sunt cupidatat veniam sunt nulla sit Lorem incididunt reprehenderit laboris aliqua proident. Quis deserunt ullamco exercitation laboris non ad amet ut. Anim voluptate ea incididunt elit non commodo anim nostrud ea amet Lorem.
      </div>
        
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
    .entry-container{
        border-bottom: 1px solid #2c3e50;
        transition: 0.2s all ease-in;

        &:hover{
            /*hcer gris con sass*/
            background-color: lighten($color: grey, $amount: 45);
            transition: 0.2s all ease-in;
        }
    }
    .entry-description{
        font-size: 12px;
    }
</style>