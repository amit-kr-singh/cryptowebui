<template>
	<div class="crypto-sidebar">
		
		<div class="sidebar d-md-none d-lg-block">
			<div class="d-flex flex-column flex-shrink-0 bg-crypto p-3" style="width: 3.5rem; height:100vh">
				<ul class="nav nav-pills nav-flush flex-column mb-auto ">
					<li class="pb-0">
					<!-- <i class="fas fa-bars"></i> -->
						<img src="icons/menu.png" alt="menu bar" height="23" />
					</li>

					<li>
						<i class="icon icon--md icon--mg-sm icon--collection"></i>
					</li>
					<li>
						<img src="icons/dashboard2.png" alt="dashboard" height="23" />
					</li>
					<li>
						<img src="icons/wallet.png" alt="wallet" height="23" />
					</li>
					<li>
						<img src="icons/chat.png" alt="chat" height="23" />
					</li>
					<li>
						<img src="icons/up-arrow.png" alt="arrow up" height="23" />
					</li>
					<li class="advertise-icon">
						<img src="icons/ad11.png" alt="add1" height="55" />
					</li>
					<li class="advertise-icon2">
						<img src="icons/advertise.png" alt="add2" height="44" />
					</li>
					<li class="advertise-icon2">
						<img src="icons/advertise2.png" alt="add2" height="44" />
					</li>
				</ul>

				<div class="">
					<div class="pb-4">
						<img src="icons/down-arrow.png" alt="arrow down" height="23" />
					</div>
					<div>
						<i class="fas fa-plus"></i>
					</div>
				</div>
			</div>
		</div>

	</div>
	
</template>

<script>
export default {
  name: 'SideBar',
};
</script>

