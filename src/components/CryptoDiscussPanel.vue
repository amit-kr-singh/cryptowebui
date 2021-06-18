<template>
	<div class="crypto-discuss-panel">
		<div class="row no-gutters">
			<div class="col-lg-12 col-md-12 p-3" style="background: rgba(0,9,19,0.2)!important;">
				<div class="row no-gutters">
					<div class="col text-center">
						<h3 class="text-white">General Discussion</h3>
					</div>
					<div class="col-lg-1 text-right">
						<img src="/icons/share.png" height="25" alt="share" />
					</div>
					<div class="col-lg-1">
						<img src="/icons/bell1.png" height="25" alt="share" />
					</div>
				</div>
			</div>
		</div>

		<div class="row no-gutters">
			<div style="max-height: 77vh;overflow: auto;">
				<div class="col-lg-12 col-md-12 mt-2 p-3 text-white">
				<div class="row no-gutters text-left" v-for="(item, index) in discussfirst" :key="index">
					<div class="col-lg-1">
						<img :src="item.url" alt="user" height="35" />
						<div class="active"></div>	
					</div>
					<div class="col-lg-9">
						<div class="font-weight-bold">
							{{item.title}}
						</div>
						<p class="h6">
							{{item.subtitle}}
						</p>
					</div>
					<div class="col text-right pt-4 m-auto">
						<p>{{item.time}}</p>
					</div>
				</div>
				<div class="row no-gutters">
					<div class="col-lg-12 border-bottom text-center">
						<p class="m-0">{{date}}</p>
					</div>
				</div>
			</div>

			<div class="col-lg-12 col-md-12 p-3 text-white">
				<div class="row no-gutters text-left " v-for="(item, index) in discusssecond" :key="index">
					<div class="col-lg-1">
						<img :src="item.url" alt="user" height="35" />
						<div class="active "></div>
					</div>
					<div class="col-lg-9">
						<div class="font-weight-bold">
							{{item.title}}
						</div>
						<section>
							<div class="row no-gutters">
								<div class="col-xs-6 col-sm-3 ">
									<img :src="item.img1"  class="image-style" /> 
								</div>
								<div class="col-xs-6 col-sm-3 ">
									<img :src="item.img2" class="image-style" />
								</div>
								<div class="col-xs-6 col-sm-3 ">
									<img :src="item.img3" class="image-style" />
								</div>
								<div class="col-xs-6 col-sm-3 ">
									<img :src="item.img4" class="image-style" />
								</div>	
							</div>
						</section>	
					</div>
					<div class="col text-right pt-4 ">
						<p>{{item.time}}</p>
					</div>
				</div>
			</div>

			<div class="col-lg-12 col-md-12 mt-2 p-3 text-white" style="background: rgba(0,9,19,0.2)!important;">
				<div class="row no-gutters text-left" v-for="(item, index) in discussthird" :key="index">
					<div class="col text-left pt-4 m-auto">
						<p>{{item.time}}</p>
					</div>
					<div class="col-lg-9 text-right">
						<div class="font-weight-bold">
							{{item.title}}
						</div>
						<p class="h6 text-left">
							{{item.subtitle}}
						</p>
					</div>
					<div class="col-lg-1">
						<div class="text-right">
							<img :src="item.url" alt="user" height="35" />
							<div class="active"></div>
						</div>	
					</div>
				</div>
			</div>

			<div class="col-lg-12 col-md-12 p-3 mt-2 text-white">
				<div class="row no-gutters text-left" v-for="(item, index) in discussfourth" :key="index">
					<div class="col-lg-1">
						<img :src="item.url" alt="user" height="35" />
						<div class="active"></div>	
					</div>
					<div class="col-lg-9">
						<div class="font-weight-bold">
							{{item.title}}
						</div>
						<p class="h6">
							{{item.subtitle}}
						</p>
					</div>
					<div class="col text-right pt-4 m-auto">
						<p>{{item.time}}</p>
					</div>
				</div>
			</div>

			<div class="col-lg-12 col-md-12 mt-2 p-3 text-white" style="background: rgba(0,9,19,0.2)!important;">
				<div class="row no-gutters text-left" v-for="(item, index) in discussfifth" :key="index">
					<div class="col text-left pt-4 m-auto">
						<p>{{item.time}}</p>
					</div>
					<div class="col-lg-9 text-right">
						<div class="font-weight-bold">
							{{item.title}}
						</div>
						<p class="h6 text-right">
							{{item.subtitle}}
						</p>
					</div>
					<div class="col-lg-1">
						<div class="text-right">
							<img :src="item.url" alt="user" height="35" />
							<div class="active"></div>
						</div>	
					</div>
				</div>
			</div>

			<div class="col-lg-12 col-md-12 p-3 mt-2 text-white">
				<div class="row no-gutters text-left" v-for="(item, index) in discussfourth" :key="index">
					<div class="col-lg-1">
						<img :src="item.url" alt="user" height="35" />
						<div class="active"></div>	
					</div>
					<div class="col-lg-9">
						<div class="font-weight-bold">
							{{item.title}}
						</div>
						<p class="h6">
							{{item.subtitle}}
						</p>
					</div>
					<div class="col text-right pt-4 m-auto">
						<p>{{item.time}}</p>
					</div>
				</div>
			</div>
			<div class="col-lg-12 col-md-12 p-3 mt-2 text-white">
				<div class="row no-gutters text-left" v-for="(item, index) in discussfourth" :key="index">
					<div class="col-lg-1">
						<img :src="item.url" alt="user" height="35" />
						<div class="active"></div>	
					</div>
					<div class="col-lg-9">
						<div class="font-weight-bold">
							{{item.title}}
						</div>
						<p class="h6">
							{{item.subtitle}}
						</p>
					</div>
					<div class="col text-right pt-4 m-auto">
						<p>{{item.time}}</p>
					</div>
				</div>
			</div>
		</div>
		<div class="col-lg-12 col-md-12 text-white" style="height: 15px;"></div>
	</div>

	</div>
</template>

<script>

export default {
  name: 'CryptoPanel',

  data(){
	return{
		date:'Today, 12/7/2017',
		discussfirst:[
			{
				url:'user1.png',
				title:'Tom Hardy',
				subtitle:'It is a long established fact that a reader will be distracted by the readable  content of a page when looking at its layout.',
				time:'2:30 PM',
			},
		],

		discusssecond:[
			{
				url:'user1.png',
				title:'Jacob Tanner',
				img1:'pic1.png',
				img2:'pic2.png',
				img3:'pic3.png',
				img4:'pic4.png',
				time:'2:30 PM',
			},
		],

		discussthird:[
			{
				time:'2:31 PM',
				title:"Viktor Bojilov",
				url:'user1.png',
				subtitle:"The textboxes shouldn't be longer than 785 px in length, just so you know. They're also 10 px from the profile picture. Don't forget, too, that they're 175 px from either edge, with the profile picture and time stamps being 30 px away from the edges. Fuzzy is 10 px split above and below.",
			},
		],

		discussfourth:[
			{
				url:'user1.png',
				title:'Jacob Tanner',
				subtitle:'It is a long established fact that a reader will be distracted by the readable  content of a page when looking at its layout.',
				time:'2:30 PM',
			},
		],

		discussfifth:[
			{
				time:'2:31 PM',
				title:"Viktor Bojilov",
				url:'user1.png',
				subtitle:"Hi Everyone! How's it going today?",
			}
		],
	}
  },
};
</script>