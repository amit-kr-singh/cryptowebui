<template>
	<div class="member-list" style="height:100%">
		
		<div class="row no-gutters bg-crypto" style="height:100%">
			<div class="col-lg-12 p-3">
				<div>
					<b-tabs content-class="mt-3">
						<b-tab title="Info" class="text-white">
							<div class="text-left">
								Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.
							</div>
						</b-tab>
						<b-tab title="Members">
							<div class="row no-gutters">
								<div class="col-lg-12 " style="margin-top: -10px;">
									<div class="input-group text-white">
										<span class="m-auto">
											<img src="icons/users.png" alt="members" height="20" />
										</span>
										<!-- <span>10,001 Members</span> -->
										<input class="form-control border-right-0" placeholder="10,001 Members">
										<span class="m-auto">
											<img src="icons/search.png" alt="search" height="20" />
										</span>
									</div>
								</div>
							</div>

							<div class="row no-gutters">
								<div class="col-lg-12 col-md-12" style="max-height:74vh; overflow:auto">
									<div class="row no-gutters">
										<div class="col-lg-12 text-left mt-3">
											<button class="accordion">Bots</button>
											<div class="accordion-content">
												<div class="row no-gutters" v-for="(item, index) in bots" :key="index">
													<div class="col-md-2">
														<img :src="item.url" alt="user" height="40" />
													</div>
													<div class="col-md-4 mt-auto mb-auto">
														{{item.title}}
													</div>
													<div class="col text-right">
														<span class="active-user"></span>
													</div>
												</div>
											</div>
										</div>

										<div class="col-lg-12 text-left">
											<button class="accordion">Owner</button>
											<div class="accordion-content">
												<div class="row no-gutters" v-for="(item, index) in owner" :key="index">
													<div class="col-md-2">
														<img :src="item.url" alt="user" height="40" />
													</div>
													<div class="col-md-4 mt-auto mb-auto">
														{{item.title}}
													</div>
													<div class="col text-right">
														<span class="not-active"></span>
													</div>
												</div>
											</div>
										</div>

										<div class="col-lg-12 text-left">
											<button class="accordion">Admins</button>
											<div class="accordion-content">
												<div class="row no-gutters mb-2" v-for="(item, index) in admin" :key="index">
													<div class="col-md-2">
														<img :src="item.url" alt="user" height="40" />
													</div>
													<div class="col-md-4 mt-auto mb-auto">
														{{item.title}}
													</div>
													<div class="col text-right">
														<span class="not-active"></span>
													</div>
												</div>
											</div>
										</div>

										<div class="col-lg-12 text-left">
											<button class="accordion">Volunteer Admins</button>
											<div class="accordion-content">
												<div class="row no-gutters mb-3" v-for="(item, index) in volunteer" :key="index">
													<div class="col-md-2">
														<img :src="item.url" alt="user" height="40" />
													</div>
													<div class="col-md-4 mt-auto mb-auto">
														{{item.title}}
													</div>
													<div class="col text-right">
														<span class="not-active"></span>
													</div>
												</div>
											</div>
										</div>
									</div>
								</div>
							</div>
						</b-tab>
						<b-tab title="Search">
							<div class="row no-gutters">
								<div class="col-lg-12 pt-1" style="margin-top: -10px;">
									<div class="input-group text-white">
										<span class="m-auto">
											<img src="icons/chat2.png" alt="members" height="20" />
										</span>
										<!-- <span>10,001 Members</span> -->
										<input class="form-control border-right-0 chat-search" placeholder="Search in this chat">
										<span class="m-auto">
											<img src="icons/search.png" alt="search" height="20" />
										</span>
									</div>
								</div>
							</div>

							<div class="row no-gutters mt-5">
								<div class="col-md-12 " style="max-height: 68vh;overflow: auto;">
									<div class="row no-gutters text-white mb-4" v-for='(item, index) in chatuser' :key="index">
										<div class="col-md-2 m-auto">
											<img :src="item.url" alt="members" height="40" />
										</div>
										<div class="col-md-10 chat-box">
											<div class="row no-gutters">
												<div class="col-md-9 text-left">
													<p class="m-0 chat-name">{{item.name}}</p>
													<p class="m-0 chat-msg">{{item.msg}}</p>
												</div>
												<div class="col-md-3">
													<p class="msg-color">{{item.time}}</p>
												</div>
											</div>
										</div>
									</div>
								</div>
							</div>
						</b-tab>
					</b-tabs>
				</div>
			</div>

			<div class="col-lg-12 mt-auto">
				<img src="logo.png" class="w-100"  alt="logo" style="height:auto" />
			</div>
		</div>

	</div>
</template>
<script>
export default {
  name: 'MemberList',

  data(){
		return{
			bots:[
				{
					url:'user2.png',
					title:'Welcome Bot',
				},
			],

			owner:[
				{
					url:'user2.png',
					title:'John Smith',
				},
			],
			admin:[
				{
					url:'user2.png',
					title:'Frank H',
				},
				{
					url:'user2.png',
					title:'Graham',
				},
				{
					url:'user2.png',
					title:'Vik',
				},
			],
			volunteer:[
				{
					url:'user2.png',
					title:'Patsy',
				},
				{
					url:'user2.png',
					title:'Jessica S',
				},
				{
					url:'user2.png',
					title:'John',
				},
				{
					url:'user2.png',
					title:'Jimi',
				},
				{
					url:'user2.png',
					title:'Handy',
				},
				{
					url:'user2.png',
					title:'Adam',
				},
			],

			chatuser:[
					{
						url:'user.png',
						name:"Jenifer Marbles",
						msg:"This as a searched for message",
						time:"11:49 AM",
					},
					{
						url:'user.png',
						name:"Marbles Jenifer ",
						msg:"This as a searched for message",
						time:"11:49 AM",
					},
					{
						url:'user.png',
						name:"Jenifer Marbles",
						msg:"This as a searched for message",
						time:"11:49 AM",
					},			
			],
		}
  }
};
</script>