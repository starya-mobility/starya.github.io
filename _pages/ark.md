---
layout: default
title: Agile Ride Kit
permalink: /ark
author: 
categories: 
tags: 
comments: false
image: 
beforetoc: ""
toc: false
---

<!-- Featured Image Full -->
<div class="wrapper">
    <section class="section-profile-cover section-shaped bgimage-container">
        <div class="shape shape-style-1 shape-primary" style="filter: brightness(0.4) grayscale();">
            <!-- Circles background -->
            <span class="span-150"></span>
            <span class="span-50"></span>
            <span class="span-50"></span>
            <span class="span-75"></span>
            <span class="span-100"></span>
            <span class="span-75"></span>
            <span class="span-50"></span>
            <span class="span-100"></span>
            <span class="span-50"></span>
            <span class="span-100"></span>
        </div>
        <div id="container" style="position: absolute;height:90vh;width: 100%;"></div>
        <div class="page-header">
            <div class="container shape-container d-flex align-items-center py-xl">
                <div class="col px-0">
                    <div class="row align-items-center justify-content-center">
                        <div class="col-lg-6 text-center">
                            <h1 class="text-white display-1">{{ page.title | strip_html | truncatewords:5 }}</h1>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- SVG separator -->
        <div class="separator separator-bottom separator-skew" style="z-index: auto;">
            <svg x="0" y="0" viewBox="0 0 2560 100" preserveAspectRatio="none" version="1.1"
                xmlns="http://www.w3.org/2000/svg">
                <polygon class="fill-secondary" points="2560 0 2560 100 0 100"></polygon>
            </svg>
        </div>
    </section>
</div>



<div class="wrapper">
  <section class="section bg-secondary">
    <div class="container">
      <div class="card card-profile shadow mt--200" style="min-height:70vh">

    
      </div>
    </div>
  </section>
</div>


<script type="text/javascript" src="{{site.url}}/assets/js/plugins/three.min.js" defer></script>
<script type="text/javascript" src="{{site.url}}/assets/js/plugins/ColladaLoader.js" defer></script>
<script type="text/javascript" src="{{site.url}}/assets/js/plugins/TrackballControls.js" defer></script>

<script type="module" defer>

    // import '{{site.url}}/assets/js/plugins/three.min.js';
    // import '{{site.url}}/assets/js/plugins/ColladaLoader.js';
    // import '{{site.url}}/assets/js/plugins/TrackballControls.js';

    var container;
    var controls, camera, scene, renderer;
    
    var angle = 0;
    var radius = 1; 

    document.addEventListener("DOMContentLoaded", function(){
                init();
            animate();
    });


    function init() {
        container = document.getElementById( 'container' );
        

        // camera = new THREE.PerspectiveCamera( 45, window.innerWidth / window.innerHeight, 0.1, 2000 );
        camera = new THREE.PerspectiveCamera( 45, $(container).width()/ $(container).height(), 0.1, 2000 );
        camera.position.set( 1, 1, 1 );
        camera.lookAt( 0, 0, 0 );

        controls = new THREE.TrackballControls( camera , container);
        controls.target.set( 0, -0.30, 0 )
        controls.enabled = false
        // controls.rotateSpeed = 1.0;
        // controls.zoomSpeed = 1.2;
        // controls.panSpeed = 0.8;
        // controls.keys = [ 65, 83, 68 ];
        

        scene = new THREE.Scene();

        var loader = new THREE.ColladaLoader();
        loader.load( '{{site.url}}/assets/starya/core.dae', function ( collada ) {
        scene.add( collada.scene );
        } );

        var ambientLight = new THREE.AmbientLight( 0xcccccc, 0.4 );
        scene.add( ambientLight );

        var directionalLight = new THREE.DirectionalLight( 0xffffff, 0.8 );
        directionalLight.position.set( 1, 1, 0 ).normalize();
        scene.add( directionalLight );

        renderer = new THREE.WebGLRenderer( { alpha: true } );
        renderer.setClearColor( 0x000000, 0 ); // the default
        renderer.setPixelRatio( window.devicePixelRatio );
        // renderer.setSize( window.innerWidth, window.innerHeight );
        renderer.setSize($(container).width(), $(container).height());
        container.appendChild(renderer.domElement);
        window.addEventListener( 'resize', onWindowResize, false );


    }

    function onWindowResize() {
        // camera.aspect = window.innerWidth / window.innerHeight;
        camera.aspect = $(container).width()/ $(container).height();
        camera.updateProjectionMatrix();
        // renderer.setSize( window.innerWidth, window.innerHeight );
        renderer.setSize($(container).width(), $(container).height());
        container.appendChild(renderer.domElement);

        controls.handleResize();
    }

    function animate() {
        requestAnimationFrame( animate );
        controls.update();
        render();

        // Use Math.cos and Math.sin to set camera X and Z values based on angle. 
        camera.position.x = radius * Math.cos( angle );  
        camera.position.z = radius * Math.sin( angle );
        angle += 0.01;
    }

    function render() {
        renderer.render( scene,camera );
    }

</script>

