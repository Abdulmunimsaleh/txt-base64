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
							<div class="card d-flex flex-wrap">
								<div class="card-body">
									<div class="row mb-4">
                                        <div class="col-sm-12 col-md-4">
											<h6 class="card-title mb-1">File Upload</h6>
										</div>
                                        <div class="col-sm-12 col-md-4">
                                            <h6 class="card-title mb-1">File Summary</h6>
										</div>
                                        <div class="col-sm-12 col-md-4">
                                            <h6 class="card-title mb-1">TXT BASE64</h6>
										</div>
									</div>
									<div class="row mb-4">
										<div class="col-sm-12 col-md-4">
											<input type="file" class="dropify" data-height="200" />
										</div>
                                        <div class="col-sm-12 col-md-4">
                                            <textarea class="form-control" placeholder="File Summary Contents" readonly="" rows="10" style="height: 139px;"></textarea>
                                            <button type="submit" class="btn btn-primary mt-4">Submit</button>
										</div>
                                        <div class="col-sm-12 col-md-4">
                                            <textarea class="form-control" placeholder="Txt base54" readonly="" rows="10" style="height: 139px;"></textarea>
										</div>
									</div>
								</div>
							</div>
						</div>
					</div>
					<!-- row closed -->
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