<template>
	<div class="crypto-panel">
		
		<div class="row no-gutters bg-crypto">
			<div class="col-lg-3">
				<CryptoPanelSidebar />
			</div>
			<div class="col-lg-9">
				<CryptoDiscussPanel />
			</div>
		</div>

	</div>
</template>
<script>
import CryptoPanelSidebar from './CryptoPanelSidebar.vue'
import CryptoDiscussPanel from './CryptoDiscussPanel.vue'
export default {
  name: 'CryptoPanel',

  components: {
    CryptoPanelSidebar,
    CryptoDiscussPanel
  }
};
</script>