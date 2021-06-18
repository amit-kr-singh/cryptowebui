<template>
  <div class="crypto-home">
        
      <div class="row no-gutters">
        <div class="col-lg-1" style="max-width: 3.5%;">
          <SideBar />
        </div>
        <div class="col-lg-11 p-3 container-fluid m-0" style="min-width: 96.2%">
          <div class="row no-gutters justify-content-between">
              <div class="col-lg-9" style="min-width: 76%;">
                <CryptoPanel />
                <div class="row no-gutters">
                  <div class="col-lg-3 text-white"></div>
                  <div class="col-lg-9 text-white mt-2">
                    <MessageBox />
                  </div>
                </div>
              </div>
              <div class="col-lg-2" style="min-width: 23.5%;">
                <MemberList />
              </div>
          </div>
        </div>
      </div>

  </div>
</template>

<script>
import SideBar from './SideBar.vue'
import CryptoPanel from './CryptoPanel.vue'
import MemberList from './MemberList.vue'
import MessageBox from './MessageBox'
export default {
  name: 'CryptoHome',

  components: {
    SideBar,
    CryptoPanel,
    MemberList,
    MessageBox
  }
};
</script>


