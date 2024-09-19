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

        <!-- Sidebar-right-->
			<div class="sidebar sidebar-right sidebar-animate">
				<div class="panel panel-primary card mb-0 box-shadow">
					<div class="tab-menu-heading border-0 p-3">
						<div class="card-title mb-0">Notifications</div>
						<div class="card-options ms-auto">
							<a href="#" class="sidebar-remove"><i class="fe fe-x"></i></a>
						</div>
					</div>
					<div class="panel-body tabs-menu-body latest-tasks p-0 border-0">
						<div class="tabs-menu ">
							<!-- Tabs -->
							<ul class="nav panel-tabs">
								<li class=""><a href="#side1" class="active" data-bs-toggle="tab"><i class="ion ion-md-chatboxes tx-18 me-2"></i> Chat</a></li>
								<li><a href="#side2" data-bs-toggle="tab"><i class="ion ion-md-notifications tx-18  me-2"></i> Notifications</a></li>
								<li><a href="#side3" data-bs-toggle="tab"><i class="ion ion-md-contacts tx-18 me-2"></i> Friends</a></li>
							</ul>
						</div>
						<div class="tab-content">
							<div class="tab-pane active " id="side1">
								<div class="list d-flex align-items-center border-bottom p-3">
									<div class="">
										<span class="avatar bg-primary brround avatar-md">CH</span>
									</div>
									<a class="wrapper w-100 ms-3" href="#" >
										<p class="mb-0 d-flex ">
											<b>New Websites is Created</b>
										</p>
										<div class="d-flex justify-content-between align-items-center">
											<div class="d-flex align-items-center">
												<i class="mdi mdi-clock text-muted me-1"></i>
												<small class="text-muted ms-auto">30 mins ago</small>
												<p class="mb-0"></p>
											</div>
										</div>
									</a>
								</div>
								<div class="list d-flex align-items-center border-bottom p-3">
									<div class="">
										<span class="avatar bg-danger brround avatar-md">N</span>
									</div>
									<a class="wrapper w-100 ms-3" href="#" >
										<p class="mb-0 d-flex ">
											<b>Prepare For the Next Project</b>
										</p>
										<div class="d-flex justify-content-between align-items-center">
											<div class="d-flex align-items-center">
												<i class="mdi mdi-clock text-muted me-1"></i>
												<small class="text-muted ms-auto">2 hours ago</small>
												<p class="mb-0"></p>
											</div>
										</div>
									</a>
								</div>
								<div class="list d-flex align-items-center border-bottom p-3">
									<div class="">
										<span class="avatar bg-info brround avatar-md">S</span>
									</div>
									<a class="wrapper w-100 ms-3" href="#" >
										<p class="mb-0 d-flex ">
											<b>Decide the live Discussion</b>
										</p>
										<div class="d-flex justify-content-between align-items-center">
											<div class="d-flex align-items-center">
												<i class="mdi mdi-clock text-muted me-1"></i>
												<small class="text-muted ms-auto">3 hours ago</small>
												<p class="mb-0"></p>
											</div>
										</div>
									</a>
								</div>
								<div class="list d-flex align-items-center border-bottom p-3">
									<div class="">
										<span class="avatar bg-warning brround avatar-md">K</span>
									</div>
									<a class="wrapper w-100 ms-3" href="#" >
										<p class="mb-0 d-flex ">
											<b>Meeting at 3:00 pm</b>
										</p>
										<div class="d-flex justify-content-between align-items-center">
											<div class="d-flex align-items-center">
												<i class="mdi mdi-clock text-muted me-1"></i>
												<small class="text-muted ms-auto">4 hours ago</small>
												<p class="mb-0"></p>
											</div>
										</div>
									</a>
								</div>
								<div class="list d-flex align-items-center border-bottom p-3">
									<div class="">
										<span class="avatar bg-success brround avatar-md">R</span>
									</div>
									<a class="wrapper w-100 ms-3" href="#" >
										<p class="mb-0 d-flex ">
											<b>Prepare for Presentation</b>
										</p>
										<div class="d-flex justify-content-between align-items-center">
											<div class="d-flex align-items-center">
												<i class="mdi mdi-clock text-muted me-1"></i>
												<small class="text-muted ms-auto">1 day ago</small>
												<p class="mb-0"></p>
											</div>
										</div>
									</a>
								</div>
								<div class="list d-flex align-items-center border-bottom p-3">
									<div class="">
										<span class="avatar bg-pink brround avatar-md">MS</span>
									</div>
									<a class="wrapper w-100 ms-3" href="#" >
										<p class="mb-0 d-flex ">
											<b>Prepare for Presentation</b>
										</p>
										<div class="d-flex justify-content-between align-items-center">
											<div class="d-flex align-items-center">
												<i class="mdi mdi-clock text-muted me-1"></i>
												<small class="text-muted ms-auto">1 day ago</small>
												<p class="mb-0"></p>
											</div>
										</div>
									</a>
								</div>
								<div class="list d-flex align-items-center border-bottom p-3">
									<div class="">
										<span class="avatar bg-purple brround avatar-md">L</span>
									</div>
									<a class="wrapper w-100 ms-3" href="#" >
										<p class="mb-0 d-flex ">
											<b>Prepare for Presentation</b>
										</p>
										<div class="d-flex justify-content-between align-items-center">
											<div class="d-flex align-items-center">
												<i class="mdi mdi-clock text-muted me-1"></i>
												<small class="text-muted ms-auto">45 minutes ago</small>
												<p class="mb-0"></p>
											</div>
										</div>
									</a>
								</div>
								<div class="list d-flex align-items-center p-3">
									<div class="">
										<span class="avatar bg-blue brround avatar-md">U</span>
									</div>
									<a class="wrapper w-100 ms-3" href="#" >
										<p class="mb-0 d-flex ">
											<b>Prepare for Presentation</b>
										</p>
										<div class="d-flex justify-content-between align-items-center">
											<div class="d-flex align-items-center">
												<i class="mdi mdi-clock text-muted me-1"></i>
												<small class="text-muted ms-auto">2 days ago</small>
												<p class="mb-0"></p>
											</div>
										</div>
									</a>
								</div>
							</div>
							<div class="tab-pane  " id="side2">
								<div class="list-group list-group-flush ">
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-lg brround cover-image" data-bs-image-src="../assets/img/faces/12.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-3">
											<strong>Madeleine</strong> Hey! there I' am available....
											<div class="small text-muted">
												3 hours ago
											</div>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-lg brround cover-image" data-bs-image-src="../assets/img/faces/1.jpg"></span>
										</div>
										<div class="ms-3">
											<strong>Anthony</strong> New product Launching...
											<div class="small text-muted">
												5 hour ago
											</div>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-lg brround cover-image" data-bs-image-src="../assets/img/faces/2.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-3">
											<strong>Olivia</strong> New Schedule Realease......
											<div class="small text-muted">
												45 minutes ago
											</div>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-lg brround cover-image" data-bs-image-src="../assets/img/faces/8.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-3">
											<strong>Madeleine</strong> Hey! there I' am available....
											<div class="small text-muted">
												3 hours ago
											</div>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-lg brround cover-image" data-bs-image-src="../assets/img/faces/11.jpg"></span>
										</div>
										<div class="ms-3">
											<strong>Anthony</strong> New product Launching...
											<div class="small text-muted">
												5 hour ago
											</div>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-lg brround cover-image" data-bs-image-src="../assets/img/faces/6.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-3">
											<strong>Olivia</strong> New Schedule Realease......
											<div class="small text-muted">
												45 minutes ago
											</div>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-lg brround cover-image" data-bs-image-src="../assets/img/faces/9.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-3">
											<strong>Olivia</strong> Hey! there I' am available....
											<div class="small text-muted">
												12 minutes ago
											</div>
										</div>
									</div>
								</div>
							</div>
							<div class="tab-pane  " id="side3">
								<div class="list-group list-group-flush ">
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/9.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Mozelle Belt</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/11.jpg"></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Florinda Carasco</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel" ><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/10.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Alina Bernier</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/2.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Zula Mclaughin</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/13.jpg"></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Isidro Heide</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/12.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Mozelle Belt</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" ><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/4.jpg"></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Florinda Carasco</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/7.jpg"></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Alina Bernier</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" ><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/2.jpg"></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Zula Mclaughin</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel" ><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/14.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Isidro Heide</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" ><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/11.jpg"></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Florinda Carasco</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/9.jpg"></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Alina Bernier</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/15.jpg"><span class="avatar-status bg-success"></span></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Zula Mclaughin</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
									<div class="list-group-item d-flex  align-items-center">
										<div>
											<span class="avatar avatar-md brround cover-image" data-bs-image-src="../assets/img/faces/4.jpg"></span>
										</div>
										<div class="ms-2">
											<div class="fw-semibold" data-bs-toggle="modal" data-bs-target="#chatmodel">Isidro Heide</div>
										</div>
										<div class="ms-auto">
											<a href="#" class="btn btn-sm btn-light" data-bs-toggle="modal" data-bs-target="#chatmodel"><i class="fab fa-facebook-messenger"></i></a>
										</div>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
			<!-- /Sidebar-right-->
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