<template>
 <div class="row items-center justify-center">
<q-card>
        <q-tabs
          v-model="tab"
          dense
          class="text-grey"
          active-color="primary"
          indicator-color="primary"
          align="justify"
          narrow-indicator
        >
          <q-tab name="user" label="User Info" />
          <q-tab name="payment" label="Request Payment" />
        </q-tabs>

        <q-separator />

        <q-tab-panels v-model="tab" animated>
          <q-tab-panel name="user" class="row justify-center">
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
          </q-tab-panel>

          <q-tab-panel name="payment" class="row justify-center">
            <div class="data-name q-mt-xl q-ml-xl">
              <div class="text">Insert your name</div>
                <q-input filled v-model="name" type="text" class="input-size q-mt-sm" label="Name" />
            </div>
            <div class="data-name q-mt-xl q-ml-xl">
                <div class="text">Insert Card number</div>
                  <q-input filled v-model="cardNumber" type="number" class="input-size q-mt-sm" label="Card Number" />
              </div>
                <div class="data-name q-mt-xl q-ml-xl">
                <div class="text">Insert Expiry Date</div>
                  <q-input filled v-model="expDate" type="number" class="input-size q-mt-sm" label="Expiry Date" />
              </div>
                  <div class="data-name q-mt-xl q-ml-xl">
                <div class="text">Insert CVV</div>
                  <q-input filled v-model="cvv" type="number" class="input-size q-mt-sm" label="CVV" />
                 </div>
          </q-tab-panel>
        </q-tab-panels>
      </q-card>
 




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
      cardNumber: '',
      expDate: '',
      cvv: '',
      tab: 'user',
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
.q-card{
  width: 100%;
}
</style>
