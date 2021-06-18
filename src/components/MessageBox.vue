<template>
	<div class="message-box bg-crypto">
		
		<div class="row no-gutters">
			<div class="col-lg-12 border-bottom">
				<div class="row no-gutters">
					<div class="col-lg-8">
						<input type="text" class="form-control" placeholder="Write message">
					</div>
					<div class="col-lg-4 text-right">
						<ul>
							<li><img src="icons/happy.png" alt="imoji" height="25" /></li>
							<li><img src="icons/picture.png" alt="picture" height="25" /></li>
							<li><img src="icons/file.png" alt="file attachment" height="25" /></li>
							<li><img src="icons/mic2.png" alt="audio" height="25" /></li>
							<li><img src="icons/left-arrow.png" alt="sent" height="25" /></li>
						</ul>
					</div>
				</div>
			</div>
		</div>

	</div>
</template>

<script>

export default {
  name: 'MessageBox',
};
</script>