---
layout: default
title: Agile Ride Kit
permalink: /ark
author: 
categories: 
tags: 
comments: false
image: https://res.cloudinary.com/gowrav/image/upload/v1588137433/Gallery%20Starya/core_sketch_at3aik.png
beforetoc: "<blockquote class='blockquote'><p class='mb-0'>The engine is the <b>heart</b> of an aeroplane and pilot its soul</p><footer class='blockquote-footer'>Walter Alexander Raleigh.</footer> </blockquote>"
toc: false
---
<!-- Featured Image -->
{% include featured-image.html %}
<div class="wrapper">
	<section class="section bg-secondary">
		<div class="container">
			<div class="card card-profile shadow mt--300">
				<div class="py-4 text-center">
					<div class="row justify-content-center">
						<div class="col-lg-9">
							<p class="lead text-muted">{{page.beforetoc}}</p>
						</div>
					</div>
				</div>
				<div class="row justify-content-center">
					<div class="col-lg-10 px-4">
						<!-- Toc if any -->{% if page.toc %}
						<div class="toc mt-4 mb-4 lead text-muted">
							<h3 class="display-3 text-warning">Summary</h3>
							{% include toc.html html=content %}</div>{% endif %}
						<!-- End Toc -->
						<!-- Main Content -->
						<div class="border-top">
							<div class="mt-5 mb-5" style="min-height: 50vh;">
								<!-- Fancy -->
								<div class="container">
									<div class="row align-items-center justify-content-center">
										<div class="col-lg-12 text-center">
											<div id="tooltip" class="btn-sm btn-primary text-uppercase" style="position: absolute;margin-top: -2rem;margin-left: -3rem;z-index: 100;display:block;visibility:hidden"></div>
											<canvas style="width:100%" id="corecontainer"></canvas>
											<div id="modalpreview"> <span class="badge badge-pill badge-success text-uppercase">Loading Preview</span>
											</div>
										</div>
									</div>
								</div>
								<!-- Motor -->
								<div class="py-5">
									<div class="container">
										<div class="row align-items-center">
											<div class="col-lg-5">
												<div class="info info-horizontal info-hover-primary">
													<div class="description">
														<h3 class="display-3 title">PMSM Motor</h3>
														<p>Permanent.Magnet.Synchronous.Motor is chosen to provide the most efficient yet completely noiseless engine for ARK core</p>
														<label>Type</label> <code>PMSM / BLAC</code>
														<br>
														<label>Continuous Power</label> <code>6.5kW</code>
														<br>
														<label>Peak Power</label> <code>10kW</code>
														<br>
														<label>Rated Speed</label> <code>2500RPM</code>
														<br>
														<label>Rated Torque</label> <code>30Nm</code>
														<br>
													</div>
												</div>
											</div>
											<div class="col-lg-7 px-5">
												<img src="https://res.cloudinary.com/gowrav/image/upload/v1588140734/Gallery%20Starya/motor_focus_iwpqzc.png" width="100%">
											</div>
										</div>
									</div>
								</div>
								<!-- Controller -->
								<div class="py-5">
									<div class="container py-5">
										<div class="row align-items-center">
											<div class="col-lg-7 px-5">
												<img src="https://res.cloudinary.com/gowrav/image/upload/v1588137433/Gallery%20Starya/controller_focus_rjmxtb.png" width="100%">
											</div>
											<div class="col-lg-5">
												<div class="info info-horizontal info-hover-primary">
													<div class="description">
														<h3 class="display-3 title">FOC Controller</h3>
														<p>With a strong open source foundation our controller runs on popular VESC architecture utilizing realtime ChibiOS to make it the most resilient motor controller for an automobile.</p>
														<label>Continuous Current</label> <code>300A</code>
														<br>
														<label>Burst Current</label> <code>450A</code>
														<br>
														<label>Control Mpde</label> <code>Field.Oriented.Control</code>
														<br>
														<label>Robustness</label> <code>Hard-Real.Time.Operating.System</code>
														<br>
													</div>
												</div>
											</div>
										</div>
									</div>
								</div>
								<!-- Power Train -->
								<div class="py-5">
									<div class="container">
										<div class="row align-items-center">
											<div class="col-lg-5">
												<div class="info info-horizontal info-hover-primary">
													<div class="description">
														<h3 class="display-3 title">Power Train</h3>
														<p>2 Pulley speed reduction power train provides the most elegant power train utlizing carbon fiber belt for efficient energy transfer</p>
														<label>Reduction Ratio</label> <code>3:1</code>
														<br>
														<label>Belt</label> <code>Carbon Fiber</code>
														<br>
														<label>Peak Torque</label> <code>120Nm+ [Consistent]</code>
														<br>
														<label>Peak Speed</label> <code>75kmph</code>
														<br>
													</div>
												</div>
											</div>
											<div class="col-lg-7 px-5">
												<img src="https://res.cloudinary.com/gowrav/image/upload/v1588137433/Gallery%20Starya/pulley_focus_foqzuk.png" width="100%">
											</div>
										</div>
									</div>
								</div>
								<!-- Cooling -->
								<div class="py-5">
									<div class="container">
										<div class="row align-items-center">
											<div class="col-lg-7 px-5">
												<img src="https://res.cloudinary.com/gowrav/image/upload/v1588139310/Gallery%20Starya/cooling_focus_aoupaq.png" width="100%">
											</div>
											<div class="col-lg-5">
												<div class="info info-horizontal info-hover-primary">
													<div class="description">
														<h3 class="display-3 title">Liquid Cooled</h3>
														<p>With great power comes great heat, and hence cooling becomes a necessity but with liquid cooling we bring not only coolness to the core but also improve its overall efficiency</p>
														<label>Method</label> <code>Radiation</code>
														<br>
														<label>Coolant</label> <code>Liquid </code>
														<br>
														<label>Rated Transfer</label> <code>200 j/s</code>
														<br>
													</div>
												</div>
											</div>
										</div>
									</div>
								</div>
								<script src="{{site.url}}/assets/3js/three.js"></script>
								<script src="{{site.url}}/assets/3js/libs/stats.min.js"></script>
								<script src="{{site.url}}/assets/3js/loaders/ColladaLoader.js"></script>
								<script src="{{site.url}}/assets/3js/controls/OrbitControls.js"></script>
								<script src="{{site.url}}/assets/3js/renderers/Projector.js"></script>
								<script>
									var canvas,tooltip,modalpreview, controls, camera, scene, renderer, core, pickHelper;
									                                    var pickPosition = {x: 0, y: 0};
									                                    function init() {
									                                        canvas = document.querySelector('#corecontainer');
									                                        tooltip = document.querySelector('#tooltip');
									                                        modalpreview = document.querySelector('#modalpreview');
									                                        renderer = new THREE.WebGLRenderer({canvas:canvas,alpha: true});
									                                        renderer.setClearColor( 0x000000, 0 ); // the default
									                                        scene = new THREE.Scene();
									                                        scene.background = new THREE.Color('white');
									                                        const fov = 45;
									                                        const aspect = 2;  // the canvas default
									                                        const near = 0.1;
									                                        const far = 100;
									                                        camera = new THREE.PerspectiveCamera(fov, aspect, near, far);
									                                        camera.position.set( 0.6, 0.1, 0.4 );
									                                        camera.lookAt( 0,0,0);
									                                        {
									                                            var ambientLight = new THREE.AmbientLight( 0xcccccc, 0.4 );
									                                            scene.add( ambientLight );
									                                            const color = 0xFFFFFF;
									                                            const intensity = 0.8;
									                                            var directionalLight = new THREE.DirectionalLight( color, intensity );
									                                            directionalLight.position.set( 1, 1, 0 ).normalize();
									                                            scene.add( directionalLight );
									                                        }
									                                        // interferese with raycaster
									                                        // var axesHelper = new THREE.AxesHelper( 5 );
									                                        // scene.add( axesHelper );
									                                        // CONTROLS
									                                        controls = new THREE.OrbitControls( camera, renderer.domElement );
									                                        controls.autoRotate = true;
									                                        controls.enableZoom  = false;
									                                        controls.enablePan  = false;
									                                        controls.enableRotate  = false;
									                                        controls.maxDistance  = 1.0;
									                                        controls.minDistance  = 0.6;
									                                        // controls.target  = new THREE.Vector3(0.38, 0.2, -0.16 );
									                                        controls.target  = new THREE.Vector3(0,0,0 );
									                                        // loading manager
									                                        var loadingManager = new THREE.LoadingManager( function () {
									                                            scene.add( core );
									                                            var motor = new THREE.Mesh( new THREE.CylinderGeometry( 0.1, 0.1,0.25, 32 ), new THREE.MeshLambertMaterial( { color: 0x0000ff,side: THREE.DoubleSide, transparent: true, opacity: 0.01 })) ;
									                                            motor.position.set(-0.11,0,0);
									                                            motor.rotation.x = Math.PI / 2;
									                                            motor.name = "motor";
									                                            scene.add( motor );
									                                            var controller = new THREE.Mesh( new THREE.BoxGeometry( 0.08, 0.08,0.18 ), new THREE.MeshLambertMaterial( { color: 0x451903,side: THREE.DoubleSide, transparent: true, opacity: 0.01 })) ;
									                                            controller.position.set(-0.4,-0.01,0);
									                                            controller.name = "controller";
									                                            scene.add( controller );
									                                            var radiator = new THREE.Mesh( new THREE.BoxGeometry( 0.08, 0.14,0.3 ), new THREE.MeshLambertMaterial( { color: 0x000023,side: THREE.DoubleSide, transparent: true, opacity: 0.01 })) ;
									                                            radiator.position.set(-0.27,-0.03,0);
									                                            radiator.name = "radiator";
									                                            scene.add( radiator );
									                                            var pulley1 = new THREE.Mesh( new THREE.CylinderGeometry( 0.1, 0.1,0.04, 32 ), new THREE.MeshLambertMaterial( { color: 0xFFFFFF,side: THREE.DoubleSide, transparent: true, opacity: 0.01 })) ;
									                                            pulley1.position.set(0.22,-0.015,0.15);
									                                            pulley1.rotation.x = Math.PI / 2;
									                                            pulley1.name = "powertrain";
									                                            scene.add( pulley1 );
									                                            var pulley2 = new THREE.Mesh( new THREE.CylinderGeometry( 0.05, 0.05,0.04, 32 ), new THREE.MeshLambertMaterial( { color: 0xFFFFFF,side: THREE.DoubleSide, transparent: true, opacity: 0.01 })) ;
									                                            pulley2.position.set(-0.11,-0.014,0.16);
									                                            pulley2.rotation.x = Math.PI / 2;
									                                            pulley2.name = "powertrain";
									                                            scene.add( pulley2 );
									                                        } );
									                                        // collada
									                                        var loader = new THREE.ColladaLoader( loadingManager );
									                                        loader.load( '{{site.url}}/assets/starya/core.dae', function ( collada ) {
									                                            core = collada.scene;
									                                            // when the mouse moves, call the given function
									                                            window.addEventListener('mousemove', setPickPosition);
									                                            window.addEventListener('mouseout', clearPickPosition);
									                                            window.addEventListener('mouseleave', clearPickPosition);
									                                            window.addEventListener('touchstart', (event) => {
									                                                // prevent the window from scrolling
									                                                //    event.preventDefault();
									                                                    setPickPosition(event.touches[0]);
									                                                }, {passive: false}
									                                            );
									                                            window.addEventListener('touchmove', (event) => {
									                                                setPickPosition(event.touches[0]);
									                                            });
									                                            window.addEventListener('touchend', clearPickPosition);
									                                            clearPickPosition();
									                                            requestAnimationFrame(render);
									                                            pickHelper = new PickHelper();
									                                        } );
									                                    }
									                                    var openmodal = function (modal) {
									                                            $("#modal-motor").modal("hide")
									                                            $("#modal-controller").modal("hide")
									                                            $("#modal-powertrain").modal("hide")
									                                            $("#modal-cooling").modal("hide")
									                                            switch(modal){
									                                                case 'motor'      :  $("#modal-motor").modal("show");break;
									                                                case 'controller' :  $("#modal-controller").modal("show");break;
									                                                case 'powertrain'     :  $("#modal-powertrain").modal("show");break;
									                                                case 'radiator'    :  $("#modal-cooling").modal("show");break;
									                                            }
									                                        };
									                                    var prepmodal = null;
									                                    class PickHelper {
									                                    constructor() {
									                                        this.raycaster = new THREE.Raycaster();
									                                        this.pickedObject = null;
									                                        this.pickedObjectSavedColor = 0;
									                                    }
									                                    pick(normalizedPosition, scene, camera, time) {
									                                            // // restore the color if there is a picked object
									                                            if (this.pickedObject) {
									                                            this.pickedObject.material.emissive.setHex(this.pickedObjectSavedColor);
									                                            this.pickedObject = undefined;
									                                            }
									                                            // cast a ray through the frustum
									                                            this.raycaster.setFromCamera(normalizedPosition, camera);
									                                            // get the list of objects the ray intersected
									                                            const intersectedObjects = this.raycaster.intersectObjects(scene.children);
									                                            if (intersectedObjects.length) {
									                                                // pick the first object. It's the closest one
									                                                this.pickedObject = intersectedObjects[0].object;
									                                                // if holding on to the same then popup modal
									                                                if(tooltip.innerHTML == this.pickedObject.name){
									                                                    if(prepmodal == null)
									                                                        prepmodal = setTimeout(openmodal, 1000, this.pickedObject.name);
									                                                }else{
									                                                    // stop modal
									                                                    if(prepmodal != null)
									                                                        clearTimeout(prepmodal);
									                                                    prepmodal = null;
									                                                }
									                                                tooltip.innerHTML = this.pickedObject.name;
									                                                tooltip.style.visibility = 'visible';
									                                                modalpreview.style.visibility = 'visible'
									                                                // save its color
									                                                this.pickedObjectSavedColor = this.pickedObject.material.emissive.getHex();
									                                                // set its emissive color to flashing red/yellow
									                                                this.pickedObject.material.emissive.setHex((time * 8) % 2 > 1 ? 0xFFFF00 : 0xFF0000);
									                                            }else{
									                                                if(prepmodal != null)
									                                                    clearTimeout(prepmodal);
									                                                prepmodal = null;
									                                                tooltip.innerHTML = "";
									                                                tooltip.style.visibility = 'hidden';
									                                                modalpreview.style.visibility = 'hidden'
									                                            }
									                                        }
									                                    }
									                                    function getCanvasRelativePosition(event) {
									                                        const rect = canvas.getBoundingClientRect();
									                                        const x = (event.clientX - rect.left) * canvas.width  / rect.width;
									                                        const y = (event.clientY - rect.top ) * canvas.height / rect.height;
									                                        if(x > 0 & y > 0 & x < (canvas.width) & y < (canvas.height))
									                                        {
									                                            tooltip.style.left = x + 'px';
									                                            tooltip.style.top = y + 'px';
									                                        }
									                                        return {
									                                            x: x,
									                                            y: y,
									                                        };
									                                    }
									                                    function setPickPosition(event) {
									                                        const pos = getCanvasRelativePosition(event);
									                                        pickPosition.x = (pos.x / canvas.width ) *  2 - 1;
									                                        pickPosition.y = (pos.y / canvas.height) * -2 + 1;  // note we flip Y
									                                    }
									                                    function clearPickPosition() {
									                                        // unlike the mouse which always has a position
									                                        // if the user stops touching the screen we want
									                                        // to stop picking. For now we just pick a value
									                                        // unlikely to pick something
									                                        pickPosition.x = -100000;
									                                        pickPosition.y = -100000;
									                                    }
									                                    function resizeRendererToDisplaySize(renderer) {
									                                        const canvas = renderer.domElement;
									                                        const width = canvas.clientWidth;
									                                        const height = canvas.clientHeight;
									                                        const needResize = canvas.width !== width || canvas.height !== height;
									                                        if (needResize) {
									                                            renderer.setSize(width, height, false);
									                                        }
									                                        return needResize;
									                                    }
									                                    function render(time) {
									                                        if (resizeRendererToDisplaySize(renderer)) {
									                                            const canvas = renderer.domElement;
									                                            camera.aspect = canvas.clientWidth / canvas.clientHeight;
									                                            camera.updateProjectionMatrix();
									                                        }
									                                        pickHelper.pick(pickPosition, scene, camera, time);
									                                        renderer.render(scene, camera);
									                                        requestAnimationFrame(render);
									                                        controls.update();
									                                    }
									                                    init();
								</script>
							</div>
						</div>
						<div class="modal fade" id="modal-motor" tabindex="-1" role="dialog" aria-labelledby="modal-notification" aria-hidden="true">
							<div class="modal-dialog modal-danger modal-dialog-centered modal-" role="document">
								<div class="modal-content bg-gradient-danger">
									<div class="modal-header">
										<h3 class="modal-title" id="modal-title-info">PMSM Motor</h3>
										<button type="button" class="close" data-dismiss="modal" aria-label="Close"> <span aria-hidden="true">×</span>
										</button>
									</div>
									<div class="modal-body">
										<div class="description">
											<p>Permanent.Magnet.Synchronous.Motor is chosen to provide the most efficient yet completely noiseless engine for ARK core</p>
											<label>Type</label> <code>PMSM / BLAC</code>
											<br>
											<label>Continuous Power</label> <code>6.5kW</code>
											<br>
											<label>Peak Power</label> <code>10kW</code>
											<br>
											<label>Rated Speed</label> <code>2500RPM</code>
											<br>
											<label>Rated Torque</label> <code>30Nm</code>
											<br>
										</div>
									</div>
								</div>
							</div>
						</div>
						<div class="modal fade" id="modal-controller" tabindex="-1" role="dialog" aria-labelledby="modal-notification" aria-hidden="true">
							<div class="modal-dialog modal-danger modal-dialog-centered modal-" role="document">
								<div class="modal-content bg-gradient-danger">
									<div class="modal-header">
										<h3 class="modal-title" id="modal-title-info">FOC Controller</h3>
										<button type="button" class="close" data-dismiss="modal" aria-label="Close"> <span aria-hidden="true">×</span>
										</button>
									</div>
									<div class="modal-body">
										<div class="description">
											<p>With a strong open source foundation our controller runs on popular VESC architecture utilizing realtime ChibiOS to make it the most resilient motor controller for an automobile.</p>
											<label>Continuous Current</label> <code>300A</code>
											<br>
											<label>Burst Current</label> <code>450A</code>
											<br>
											<label>Control Mpde</label> <code>Field.Oriented.Control</code>
											<br>
											<label>Robustness</label> <code>Hard-Real.Time.Operating.System</code>
											<br>
										</div>
									</div>
								</div>
							</div>
						</div>
						<div class="modal fade" id="modal-powertrain" tabindex="-1" role="dialog" aria-labelledby="modal-notification" aria-hidden="true">
							<div class="modal-dialog modal-danger modal-dialog-centered modal-" role="document">
								<div class="modal-content bg-gradient-danger">
									<div class="modal-header">
										<h3 class="modal-title" id="modal-title-info">Power Train</h3>
										<button type="button" class="close" data-dismiss="modal" aria-label="Close"> <span aria-hidden="true">×</span>
										</button>
									</div>
									<div class="modal-body">
										<div class="description">
											<p>2 Pulley speed reduction power train provides the most elegant power train utlizing carbon fiber belt for efficient energy transfer</p>
											<label>Reduction Ratio</label> <code>3:1</code>
											<br>
											<label>Belt</label> <code>Carbon Fiber</code>
											<br>
											<label>Peak Torque</label> <code>120Nm+ [Consistent]</code>
											<br>
											<label>Peak Speed</label> <code>75kmph</code>
											<br>
										</div>
									</div>
								</div>
							</div>
						</div>
						<div class="modal fade" id="modal-cooling" tabindex="-1" role="dialog" aria-labelledby="modal-notification" aria-hidden="true">
							<div class="modal-dialog modal-danger modal-dialog-centered modal-" role="document">
								<div class="modal-content bg-gradient-danger">
									<div class="modal-header">
										<h3 class="modal-title" id="modal-title-info">Liquid Cooled</h3>
										<button type="button" class="close" data-dismiss="modal" aria-label="Close"> <span aria-hidden="true">×</span>
										</button>
									</div>
									<div class="modal-body">
										<div class="description">
											<p>With great power comes great heat, and hence cooling becomes a necessity but with liquid cooling we bring not only coolness to the core but also improve its overall efficiency</p>
											<label>Method</label> <code>Radiation</code>
											<br>
											<label>Coolant</label> <code>Liquid </code>
											<br>
											<label>Rated Transfer</label> <code>200 j/s</code>
											<br>
										</div>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</div>