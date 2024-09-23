<template>
	<div class="main-body app sidebar-mini">
        <!-- Loader -->
		<div id="global-loader">
			<img src="../assets/img/loader.svg" class="loader-img" alt="Loader">
		</div>
		<!-- /Loader -->

		<!-- Page -->
		<div class="page">

        <!-- main-content -->
        <div class='main-content app-content'>
            <div class="container-fluid">

					<!-- row -->
					<div class="row main-content-app mb-4 mt-5">
						<div class="col-xl-8 col-lg-7 mt-5">
							<div class="card mt-5">
								<a class="main-header-arrow" href="#" id="ChatBodyHide"><i class="icon ion-md-arrow-back"></i></a>
								<div class="main-content-body">
									<div class="main-chat-header">
										<div class="main-img-user"><img alt="" src="../assets/img/faces/9.jpg"></div>
										<div class="main-chat-msg-name">
											<h6>Chatbot</h6><small>Online</small>
										</div>
									</div><!-- main-chat-header -->
									<div class="main-chat-body overflow-auto" id="ChatBody">
										<div class="content-inner">
											<label class="main-chat-time"><span>3 days ago</span></label>
											<div class="media flex-row-reverse">
												<div class="main-img-user online"><img alt="" src="../assets/img/faces/9.jpg"></div>
												<div class="media-body">
													<div class="main-msg-wrapper right">
														Nulla consequat massa quis enim. Donec pede justo, fringilla vel...
													</div>
													<div class="main-msg-wrapper right">
														rhoncus ut, imperdiet a, venenatis vitae, justo...
													</div>
													<div class="main-msg-wrapper pd-0"><img alt="" class="wd-100 ht-100" src="../assets/img/ecommerce/01.jpg"></div>
													<div>
														<span>9:48 am</span> <a href="#"><i class="icon ion-android-more-horizontal"></i></a>
													</div>
												</div>
											</div>
											<div class="media">
												<div class="main-img-user online"><img alt="" src="../assets/img/faces/6.jpg"></div>
												<div class="media-body">
													<div class="main-msg-wrapper left">
														Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.
													</div>
													<div>
														<span>9:32 am</span> <a href="#"><i class="icon ion-android-more-horizontal"></i></a>
													</div>
												</div>
											</div>
											<div class="media flex-row-reverse">
												<div class="main-img-user online"><img alt="" src="../assets/img/faces/9.jpg"></div>
												<div class="media-body">
													<div class="main-msg-wrapper right">
														Nullam dictum felis eu pede mollis pretium
													</div>
													<div>
														<span>11:22 am</span> <a href="#"><i class="icon ion-android-more-horizontal"></i></a>
													</div>
												</div>
											</div><label class="main-chat-time"><span>Yesterday</span></label>
											<div class="media">
												<div class="main-img-user online"><img alt="" src="../assets/img/faces/6.jpg"></div>
												<div class="media-body">
													<div class="main-msg-wrapper left">
														Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.
													</div>
													<div>
														<span>9:32 am</span> <a href="#"><i class="icon ion-android-more-horizontal"></i></a>
													</div>
												</div>
											</div>
											<div class="media flex-row-reverse">
												<div class="main-img-user online"><img alt="" src="../assets/img/faces/9.jpg"></div>
												<div class="media-body">
													<div class="main-msg-wrapper right">
														Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo.
													</div>
													<div class="main-msg-wrapper right">
														Nullam dictum felis eu pede mollis pretium
													</div>
													<div>
														<span>9:48 am</span> <a href="#"><i class="icon ion-android-more-horizontal"></i></a>
													</div>
												</div>
											</div><label class="main-chat-time"><span>Today</span></label>
											<div class="media">
												<div class="main-img-user online"><img alt="" src="../assets/img/faces/6.jpg"></div>
												<div class="media-body">
													<div class="main-msg-wrapper left">
														Maecenas tempus, tellus eget condimentum rhoncus
													</div>
													<div class="main-msg-wrapper left">
														Nam quam nunc, blandit vel, luctus pulvinar, hendrerit id, lorem. Maecenas nec odio et ante tincidunt tempus. Donec vitae sapien ut libero venenatis faucibus.
													</div>
													<div>
														<span>10:12 am</span> <a href="#"><i class="icon ion-android-more-horizontal"></i></a>
													</div>
												</div>
											</div>
											<div class="media flex-row-reverse">
												<div class="main-img-user online"><img alt="" src="../assets/img/faces/9.jpg"></div>
												<div class="media-body">
													<div class="main-msg-wrapper right">
														Maecenas tempus, tellus eget condimentum rhoncus
													</div>
													<div class="main-msg-wrapper right">
														Nam quam nunc, blandit vel, luctus pulvinar, hendrerit id, lorem. Maecenas nec odio et ante tincidunt tempus. Donec vitae sapien ut libero venenatis faucibus.
													</div>
													<div>
														<span>09:40 am</span> <a href="#"><i class="icon ion-android-more-horizontal"></i></a>
													</div>
												</div>
											</div>
										</div>
									</div>
								</div>
								<div class="main-chat-footer">
									<nav class="nav">
										<a class="nav-link" data-bs-toggle="tooltip" href="#" title="Add Photo"><i class="fas fa-camera"></i></a> <a class="nav-link" data-bs-toggle="tooltip" href="#" title="Attach a File"><i class="fas fa-paperclip"></i></a> <a class="nav-link" data-bs-toggle="tooltip" href="#" title="Add Emoticons"><i class="far fa-smile"></i></a> <a class="nav-link" href="#"><i class="fas fa-ellipsis-v"></i></a>
									</nav><input class="form-control" placeholder="Type your message here..." type="text"> <a class="main-msg-send" href="#"><i class="far fa-paper-plane"></i></a>
								</div>
							</div>
						</div>
					</div>
					<!-- row -->
            </div>
            <!-- Container closed -->
        </div>
        <!-- main-content closed -->
        <!-- Footer opened -->
			<div class="main-footer ht-40">
				<div class="container-fluid pd-t-0-f ht-100p">
					<span>Copyright © 2021 <a href="#">Valex</a>. Designed by <a href="https://www.spruko.com/">Spruko</a> All rights reserved.</span>
				</div>
			</div>
			<!-- Footer closed -->
        
        </div>
	</div>
</template>