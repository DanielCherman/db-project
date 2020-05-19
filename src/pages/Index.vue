<template>
 <div class="row items-center justify-center">
   <div class="data-name q-mt-xl q-ml-xl">
     <div class="text">Insert your name</div>
      <q-input filled v-model="name" type="text" class="input-size q-mt-sm" label="Name" />
   </div>
   <div class="data-name q-mt-xl q-ml-xl">
     <div class="text">Insert your address</div>
      <q-input filled v-model="address" type="text" class="input-size q-mt-sm" label="Address" />
   </div>
   <div class="data-name q-mt-xl q-ml-xl">
     <div class="text">Insert Phone Number</div>
      <q-input filled v-model="phone" type="text" class="input-size q-mt-sm" mask="+370########" label="Phone" />
   </div>
   <div class="data-name q-mt-xl q-ml-xl">
     <div class="text">Insert Post Code</div>
      <q-input filled v-model="post" type="text" class="input-size q-mt-sm" mask="#####" label="Post" />
   </div>
    <div class="data-name q-mt-xl q-ml-xl">
     <div class="text">Insert Email</div>
      <q-input filled v-model="email" type="email" class="input-size q-mt-sm" label="Email" />
   </div>




 </div>
</template>

<script>
export default {
  data(){
    return{
      name: '',
      address: '',
      phone: '',
      post: '',
      email: '',
    }
  }
}
</script>
<style lang="scss">
.input-size{
  width: 400px;
}
.text{
  font-size: 25px;
}
</style>