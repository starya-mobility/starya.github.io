---
layout: page
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
<!-- Fancy -->
<div class="container">
    <div class="row align-items-center justify-content-center">
        <div class="col-lg-10 text-center" id="corecontainer" style="height:40vh;"></div>
        <!-- <div class="col-md-4">
            <button type="button" class="btn btn-block btn-warning mb-3" data-toggle="modal" data-target="#modal-notification">Notification</button>    
        </div>
        -->
        <div class="modal fade" id="modal-motor" tabindex="-1" role="dialog" aria-labelledby="modal-notification" aria-hidden="true">
                <div class="modal-dialog modal-danger modal-dialog-centered modal-" role="document">
                <div class="modal-content bg-gradient-danger">
                    <div class="modal-header">
                    <h3 class="modal-title" id="modal-title-info">PMSM Motor</h3>
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">×</span>
                    </button>
                    </div>
                    <div class="modal-body">
                        <div class="description">
                        <p>Permanent.Magnet.Synchronous.Motor is chosen to provide the most efficient yet completely noiseless engine for ARK core</p>
                        <label>Type</label>
                        <code>PMSM / BLAC</code>
                        <br>
                        <label>Continuous Power</label>
                        <code>6.5kW</code>
                        <br>
                        <label>Peak Power</label>
                        <code>10kW</code>
                        <br>
                        <label>Rated Speed</label>
                        <code>2500RPM</code>
                        <br>
                        <label>Rated Torque</label>
                        <code>30Nm</code>
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
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">×</span>
                    </button>
                    </div>
                        <div class="modal-body">
                            <div class="description">
                            <p>With a strong open source foundation our controller runs on popular VESC architecture utilizing realtime ChibiOS to make it the most resilient motor controller for an automobile.</p>
                            <label>Continuous Current</label>
                            <code>300A</code>
                            <br>
                            <label>Burst Current</label>
                            <code>450A</code>
                            <br>
                            <label>Control Mpde</label>
                            <code>Field.Oriented.Control</code>
                            <br>
                            <label>Robustness</label>
                            <code>Hard-Real.Time.Operating.System</code>
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
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">×</span>
                    </button>
                    </div>
                        <div class="modal-body">
                            <div class="description">
                            <p>2 Pulley speed reduction power train provides the most elegant power train utlizing carbon fiber belt for efficient energy transfer</p>
                            <label>Reduction Ratio</label>
                            <code>3:1</code>
                            <br>
                            <label>Belt</label>
                            <code>Carbon Fiber</code>
                            <br>
                            <label>Peak Torque</label>
                            <code>120Nm+ [Consistent]</code>
                            <br>
                            <label>Peak Speed</label>
                            <code>75kmph</code>
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
                    <button type="button" class="close" data-dismiss="modal" aria-label="Close">
                        <span aria-hidden="true">×</span>
                    </button>
                    </div>
                        <div class="modal-body">
                            <div class="description">
                            <p>With great power comes great heat, and hence cooling becomes a necessity but with liquid cooling we bring not only coolness to the core but also improve its overall efficiency</p>
                            <label>Method</label>
                            <code>Radiation</code>
                            <br>
                            <label>Coolant</label>
                            <code>Liquid </code>
                            <br>
                            <label>Rated Transfer</label>
                            <code>200 j/s</code>
                            <br>
                        </div>
                    </div>
                </div>
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
                        <label>Type</label>
                        <code>PMSM / BLAC</code>
                        <br>
                        <label>Continuous Power</label>
                        <code>6.5kW</code>
                        <br>
                        <label>Peak Power</label>
                        <code>10kW</code>
                        <br>
                        <label>Rated Speed</label>
                        <code>2500RPM</code>
                        <br>
                        <label>Rated Torque</label>
                        <code>30Nm</code>
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
                        <label>Continuous Current</label>
                        <code>300A</code>
                        <br>
                        <label>Burst Current</label>
                        <code>450A</code>
                        <br>
                        <label>Control Mpde</label>
                        <code>Field.Oriented.Control</code>
                        <br>
                        <label>Robustness</label>
                        <code>Hard-Real.Time.Operating.System</code>
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
                        <label>Reduction Ratio</label>
                        <code>3:1</code>
                        <br>
                        <label>Belt</label>
                        <code>Carbon Fiber</code>
                        <br>
                        <label>Peak Torque</label>
                        <code>120Nm+ [Consistent]</code>
                        <br>
                        <label>Peak Speed</label>
                        <code>75kmph</code>
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
                        <label>Method</label>
                        <code>Radiation</code>
                        <br>
                        <label>Coolant</label>
                        <code>Liquid </code>
                        <br>
                        <label>Rated Transfer</label>
                        <code>200 j/s</code>
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
    // import * as THREE from '{{site.url}}/assets/build/three.module.js';
    // import Stats from '{{site.url}}/assets/jsm/libs/stats.module.js';
    // import { ColladaLoader } from '{{site.url}}/assets/jsm/loaders/ColladaLoader.js';
    // import { OrbitControls } from '{{site.url}}/assets/jsm/controls/OrbitControls.js';
    // import { Projector } from '{{site.url}}/assets/jsm/renderers/Projector.js';

    var container, controls, stats, clock;
    var camera, scene, renderer, core;

    var projector, mouse = { x: 0, y: 0 };
    init();
    animate();

    function init() {

        corecontainer = document.getElementById('corecontainer');
        scene = new THREE.Scene();
        clock = new THREE.Clock();
        camera = new THREE.PerspectiveCamera( 45, corecontainer.clientWidth / corecontainer.clientHeight, 0.1, 2000 );
        camera.position.set( 0.6, 0.2, 0.4 );
        camera.lookAt( 0,0,0);
    
        // interferese with raycaster
        // var axesHelper = new THREE.AxesHelper( 5 );
        // scene.add( axesHelper );

        renderer = new THREE.WebGLRenderer( { alpha: true } );
        renderer.setClearColor( 0x000000, 0 ); // the default
        renderer.setPixelRatio( window.devicePixelRatio );
        // renderer.setSize( window.innerWidth, window.innerHeight );
        renderer.setSize(corecontainer.clientWidth, corecontainer.clientHeight);
        corecontainer.appendChild( renderer.domElement );
        
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

            var motor = new THREE.Mesh( new THREE.CylinderGeometry( 0.13, 0.13,0.25, 32 ), new THREE.MeshBasicMaterial( { color: 0x0000ff,side: THREE.DoubleSide, transparent: true, opacity: 1.0 })) ;
            motor.position.set(-0.11,0,0);
            motor.rotation.x = Math.PI / 2;
            motor.name = "motor";
            scene.add( motor );

            var controller = new THREE.Mesh( new THREE.BoxGeometry( 0.08, 0.08,0.18 ), new THREE.MeshBasicMaterial( { color: 0x451903,side: THREE.DoubleSide, transparent: true, opacity: 1.0 })) ;
            controller.position.set(-0.4,0,0);
            controller.name = "controller";
            scene.add( controller );

            var cooling = new THREE.Mesh( new THREE.BoxGeometry( 0.08, 0.14,0.3 ), new THREE.MeshBasicMaterial( { color: 0x000023,side: THREE.DoubleSide, transparent: true, opacity: 1.0 })) ;
            cooling.position.set(-0.27,-0.03,0);
            cooling.name = "cooling";
            scene.add( cooling );

            var pulley1 = new THREE.Mesh( new THREE.CylinderGeometry( 0.1, 0.1,0.04, 32 ), new THREE.MeshBasicMaterial( { color: 0xFFFFFF,side: THREE.DoubleSide, transparent: true, opacity: 1.0 })) ;
            pulley1.position.set(0.22,-0.015,0.15);
            pulley1.rotation.x = Math.PI / 2;
            pulley1.name = "pulley";
            scene.add( pulley1 );

            var pulley2 = new THREE.Mesh( new THREE.CylinderGeometry( 0.05, 0.05,0.04, 32 ), new THREE.MeshBasicMaterial( { color: 0xFFFFFF,side: THREE.DoubleSide, transparent: true, opacity: 1.0 })) ;
            pulley2.position.set(-0.11,-0.015,0.16);
            pulley2.rotation.x = Math.PI / 2;
            pulley2.name = "pulley";
            scene.add( pulley2 );

        } );

        // collada

        var loader = new THREE.ColladaLoader( loadingManager );

        loader.load( '{{site.url}}/assets/starya/core.dae', function ( collada ) {
            core = collada.scene;
        } );

        //
        var ambientLight = new THREE.AmbientLight( 0xcccccc, 0.4 );
        scene.add( ambientLight );

        var directionalLight = new THREE.DirectionalLight( 0xffffff, 0.8 );
        directionalLight.position.set( 1, 1, 0 ).normalize();
        scene.add( directionalLight );

        //

        // stats = new Stats();
        // corecontainer.appendChild( stats.dom );

        //

        window.addEventListener( 'resize', onWindowResize, false );
        
        // initialize object to perform world/screen calculations
        projector = new THREE.Projector();
        
        // when the mouse moves, call the given function
        document.addEventListener( 'mousedown', onDocumentMouseDown, false );
        // document.addEventListener( 'mousemove', onDocumentMouseMove, false );
    }

    function onWindowResize() {

        camera.aspect = corecontainer.clientWidth / corecontainer.clientHeight;
        camera.updateProjectionMatrix();
        renderer.setSize(corecontainer.clientWidth, corecontainer.clientHeight);

    }
    
    function onDocumentMouseDown( event ) 
    {
        // update the mouse variable
        mouse.x = ( event.clientX / window.innerWidth ) * 2 - 1;
        mouse.y = - ( event.clientY / window.innerHeight ) * 2 + 1;
        
        // find intersections

        // create a Ray with origin at the mouse position
        //   and direction into the scene (camera direction)
        var vector = new THREE.Vector3( mouse.x, mouse.y, 1 );
        projector.unprojectVector( vector, camera );

        var ray = new THREE.Raycaster( camera.position, vector.sub( camera.position ).normalize() );

        // create an array containing all objects in the scene with which the ray intersects
        var intersects = ray.intersectObjects( scene.children);
        // if there is one (or more) intersections
        if (intersects.length) {
        // intersections are, by default, ordered by distance,
        // so we only care for the first one. The intersection
        // object holds the intersection point, the face that's
        // been "hit" by the ray, and the object to which that
        // face belongs. We only care for the object itself.
        var target = intersects[0].object;
        console.log(target.name);

        $('#modal-motor').modal('hide');
        $('#modal-controller').modal('hide');
        $('#modal-powertrain').modal('hide');
        $('#modal-cooling').modal('hide');

        if(target.name == 'motor')
            $('#modal-motor').modal('show');
        if(target.name == 'controller')
            $('#modal-controller').modal('show');
        if(target.name == 'pulley')
            $('#modal-powertrain').modal('show');
        if(target.name == 'cooling')
            $('#modal-cooling').modal('show');

        }

    }
    
    function animate() {
        requestAnimationFrame( animate );
        render();
        controls.update();
        // stats.update();
    }

    function render() {
        var delta = clock.getDelta();
        renderer.render( scene, camera );
    }

</script>