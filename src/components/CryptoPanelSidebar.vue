<template>
	<div class="crypto-panel-sidebar">
		
		<div class="row no-gutters justify-content-center">
			<div class="col-lg-12 col-md-12">
				<div class="row no-gutters p-3">
					<div class="col-lg-12 col-md-12">
						<h3 class="text-white">Eidoo</h3>
					</div>
					<div class="col-lg-12 col-md-12">
						<ul>
							<li><a href="#"><img src="/icons/check-mark.png" height="20" /></a></li>
							<li><a href="#"><img src="/icons/home.png" height="20" /></a></li>
							<li><a href="#"><img src="/icons/settings.png" height="20" /></a></li>
						</ul>
					</div>
				</div>

				<div class="row no-gutters" >
					<div class="col-lg-12 col-md-12 text-left" id="eido" style="height:74vh; overflow:auto;">
						<button class="accordion">Public Channels</button>
						<div class="accordion-content">
							<div class="row no-gutters mb-4 crypto-select" >
								<div class="col-md-2 m-auto">
									<div>
										<img :src="publicgeneral.url" height="24" />
									</div>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{publicgeneral.title}}</p>
									<p class="sub-title">{{publicgeneral.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{publicgeneral.time}}</p>
								</div>
							</div>

							<div class="row no-gutters mb-4 crypto-select" >
								<div class="col-md-2 m-auto">
									<p class="round-pill m-auto">{{publicbounty.count}}</p>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{publicbounty.title}}
										<span>
											<img src="/icons/bell2.png" height="15" alt="share" />
										</span>
									</p>
									<p class="sub-title">{{publicbounty.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{publicbounty.time}}</p>
								</div>
							</div>

							<div class="row no-gutters mb-4 crypto-select" >
								<div class="col-md-2 m-auto">
									<p class="round-pill">{{publicprice.count}}</p>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{publicprice.title}}
										<span>
											<img src="/icons/bell2.png" height="15" alt="share" />
										</span>
									</p>
									<p class="sub-title">{{publicprice.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{publicprice.time}}</p>
								</div>
							</div>

							<div class="row no-gutters mb-4 crypto-select" >
								<div class="col-md-2 text-center m-auto">
									<p class="count-support">{{publicsupport.count}}</p>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{publicsupport.title}}</p>
									<p class="sub-title">{{publicsupport.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{publicsupport.time}}</p>
								</div>
							</div>
						</div>
							
						<button class="accordion">Website Development</button>
						<div class="accordion-content">
							<div class="row no-gutters mb-4" v-for="(item, index) in websiteitems" :key="index">
								<div class="col-md-2 m-auto">
									<div>
										<img :src="item.url" height="24" />
									</div>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{item.title}}</p>
									<p class="sub-title">{{item.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{item.time}}</p>
								</div>
							</div>
						</div>

						<button class="accordion">Project Development</button>
						<div class="accordion-content">
							<div class="row no-gutters mb-4" >
								<div class="col-md-2 m-auto">
									<div>
										<img :src="projectfirst.url" height="20" />
									</div>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{projectfirst.title}}</p>
									<p class="sub-title">{{projectfirst.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{projectfirst.time}}</p>
								</div>
							</div>

							<div class="row no-gutters mb-4" >
								<div class="col-md-2 m-auto">
									<p class="project-symbol">{{projectsecond.symbol}}</p>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{projectsecond.title}}</p>
									<p class="sub-title">{{projectsecond.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{projectsecond.time}}</p>
								</div>
							</div>

							<div class="row no-gutters mb-4" >
								<div class="col-md-2 m-auto">
									<p class="quality-pill">{{projectthird.count}}</p>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{projectthird.title}}</p>
									<p class="sub-title">{{projectthird.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{projectthird.time}}</p>
								</div>
							</div>
						</div>

						<button class="accordion">Management</button>
						<div class="accordion-content">
							<div class="row no-gutters mb-4" >
								<div class="col-md-2 m-auto">
									<img :src="managementfirst.url" height="20" />
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{managementfirst.title}}</p>
									<p class="sub-title">{{managementfirst.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{managementfirst.time}}</p>
								</div>
							</div>

							<div class="row no-gutters mb-4" >
								<div class="col-md-2 m-auto">
									<p>{{managementsecond.symbol}}</p>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{managementsecond.title}}</p>
									<p class="sub-title">{{managementsecond.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{managementsecond.time}}</p>
								</div>
							</div>

							<div class="row no-gutters mb-4" >
								<div class="col-md-2 m-auto">
									<p>{{managementthird.count}}</p>
								</div>
								<div class="col-md-7 pl-3">
									<p class="title-head">{{managementthird.title}}</p>
									<p class="sub-title">{{managementthird.subtitle}}</p>
								</div>
								<div class="col-md-3 m-auto text-right">
									<p class="time">{{managementthird.time}}</p>
								</div>
							</div>
						</div>
					</div>
					
				</div>
			</div>	
		</div>

	</div>
</template>
<script>
export default {
  name: 'CryptoPanelSidebar',

	data(){
		return{
			publicgeneral:
				{
					url:'/icons/double-check.png',
					title: 'General Discussion',
					subtitle: 'You: Hi everyone! How...',
					time: 'Just now',
				},
			publicbounty:
				{
					count: "1.1k",
					title: 'Bounty Program',
					subtitle: 'Jamie: Hi everyone! How...',
					time: '12:19 AM',
				},
			publicprice:
				{
					count: '5.3k',
					title: 'Price/Typing',
					subtitle: 'Graham: Hi everyone! How...',
					time: '6:01 PM',
				},
			publicsupport:
				{
					count: '1',
					title: 'Support',
					subtitle: 'Graham: Hi everyone! How...',
					time: '6:01 PM',
				},



			websiteitems:[
				{
					url:'/icons/double-check.png',
					title:"UI/UX Designer",
					subtitle:"Graham: Hi Developer...",
					time:'6:05PM',
				},
				{
					url:'/icons/double-check.png',
					title:"UI/UX Designer",
					subtitle:"John: Hi Developer...",
					time:'6:05PM',
				},
				{
					url:'/icons/double-check.png',
					title:"UI/UX Designer",
					subtitle:"Jacob: Hi Developer...",
					time:'6:05PM',
				},
			],

			projectfirst:
				{
					url:'/icons/tick.png',
					title:"Engineering",
					subtitle:"You: Hi Developer...",
					time:'6:05PM',
				},
			projectsecond:
				{
					symbol:'@',
					title:"R&D",
					subtitle:"You: Hi Developer...",
					time:'6:05PM',
				},
			projectthird:
				{
					count:'80',
					title:"Quality Typing",
					subtitle:"Simon: Hi Developer...",
					time:'6:05PM',
				},
			

			managementfirst:
				{
					url:'/icons/tick.png',
					title:"HR",
					subtitle:"You: Hi Developer...",
					time:'6:05PM',
				},
			managementsecond:
				{
					symbol:'@',
					title:"Operation Manager",
					subtitle:"You: Hi Developer...",
					time:'6:05PM',
				},
			managementthird:
				{
					count:'80',
					title:"MD",
					subtitle:"Simon: Hi Developer...",
					time:'6:05PM',
				},
			
		}
  }
};
</script>