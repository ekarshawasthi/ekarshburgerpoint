(function($) {  

    /*-------------------------------------
       Home page main Slider
       -------------------------------------*/
    $(document).ready(function (){
      // Declare Carousel jquery object
      var owl = $('#main-slider');

      // Carousel initialization
      owl.owlCarousel({
          loop:true,
          margin:0,
          navSpeed:800,
          nav:true,
          navText: ["<i class='fa fa-angle-left'></i>", "<i class='fa fa-angle-right'></i>"],
          items:1,
          autoplay:true,
          transitionStyle : "fade",
      });

      // add animate.css class(es) to the elements to be animated
      function setAnimation ( _elem, _InOut ) {
        // Store all animationend event name in a string.
        // cf animate.css documentation
        var animationEndEvent = 'webkitAnimationEnd mozAnimationEnd MSAnimationEnd oanimationend animationend';

        _elem.each ( function () {
          var $elem = $(this);
          var $animationType = 'animated ' + $elem.data( 'animation-' + _InOut );

          $elem.addClass($animationType).one(animationEndEvent, function () {
            $elem.removeClass($animationType); // remove animate.css Class at the end of the animations
          });
        });
      }

    // Fired before current slide change
      owl.on('change.owl.carousel', function(event) {
          var $currentItem = $('.owl-item', owl).eq(event.item.index);
          var $elemsToanim = $currentItem.find("[data-animation-out]");
          setAnimation ($elemsToanim, 'out');
      });

    // Fired after current slide has been changed
      owl.on('changed.owl.carousel', function(event) {

          var $currentItem = $('.owl-item', owl).eq(event.item.index);
          var $elemsToanim = $currentItem.find("[data-animation-in]");
          setAnimation ($elemsToanim, 'in');
      })
});


 /*-------------------------------
    Slider js
    ---------------------------------*/  
    $('.slider-of-chef').slick({
       slidesToShow: 1,
       slidesToScroll: 1,
       arrows: false,
       fade: true,
       asNavFor: '.slider-nav'
     });
     $('.slider-nav').slick({
       slidesToShow: 4,
       slidesToScroll: 1,
       asNavFor: '.slider-of-chef',
       dots: false,
       focusOnSelect: true,
       centerMode:true,
       centerPadding: '0',
     });


    /*----------------------------
    Testimonial js active
    ------------------------------ */

     $('.testimonials').slick({
       slidesToShow: 1,
       slidesToScroll: 1,
       arrows: false,
       fade: true,
       asNavFor: '.testimonials-nav'
     });
     $('.testimonials-nav').slick({
       slidesToShow: 3,
       slidesToScroll: 1,
       asNavFor: '.testimonials',
       dots: true,
       focusOnSelect: true,
       centerMode:true,
       centerPadding: '0',
     });

   /*-------------------------------------
       Menu Gallery jQuery activation code
    -------------------------------------*/
    if($(".menu-gallery").length){
      $(".menu-gallery").owlCarousel({
          // Most important owl features
          items : 4,  
          nav: true,
          navText: false,  
          dots: false,
          loop: true,
          autoplay: false,
          // Responsive options
          responsive: true,
          responsive:{
          0:{
            items:1, // In this configuration 1 is enabled from 0px up to 479px screen size
            nav: false, // from 480 to max 
            dots: true,
          },
          600:{
            items:2, // from this breakpoint 678 to 959
            nav: false, // from 480 to max 
            dots: true,
          },
          960:{

            items:4, // from this breakpoint 960 to 1199
            margin:20, // and so on...
            center:false, 

          },

          1200:{

            items:4,
            margin: 0,

          }
        } 
      });
    }

   /*-------------------------------------
       One Page Nav Scroll
    -------------------------------------*/

    $(".rs-menu li").on("click", function () {
        if ($(".showhide").is(":visible")) {
            $(".showhide").trigger("click");
        }
    });
    if ($.fn.onePageNav) {
        $(".nav-menu").onePageNav({
            currentClass: "active"
        });
    }

  /*-------------------------------------
       blog-gallery jQuery activation code
    -------------------------------------*/
    if($(".blog-gallery").length){
      $(".blog-gallery").owlCarousel({
          // Most important owl features
          items : 3,  
          nav: true,
          navText: false,
          margin: 30,  
          dots: false,
          loop: true,
          autoplay: true,
          // Responsive options
          responsive: true,
          responsive:{
          0:{
            items:1, // In this configuration 1 is enabled from 0px up to 479px screen size
            nav: false, // from 480 to max 
            dots: true,
          },
          600:{
            items:2, // from this breakpoint 678 to 959
            nav: false, // from 480 to max 
            dots: true,
          },
          960:{

            items:3, // from this breakpoint 960 to 1199
            margin:20, // and so on...
            center:false, 

          },

          1200:{

            items:3,
            margin: 30,

          }
        } 
      });
    }

    /*-------------------------------------
       blog-gallery jQuery activation code
    -------------------------------------*/
    if($(".chef-gallery").length){
      $(".chef-gallery").owlCarousel({
          // Most important owl features
          items : 3,  
          nav: true,
          navText: false,
          margin: 25,  
          dots: false,
          loop: true,
          autoplay: true,
          // Responsive options
          responsive: true,
          responsive:{
          0:{
            items:1, // In this configuration 1 is enabled from 0px up to 479px screen size
            nav: false, // from 480 to max 
            dots: true,
            margin:10,
          },
          600:{
            items:2, // from this breakpoint 678 to 959
            nav: false, // from 480 to max 
            dots: true,
            margin:10,
          },
          960:{

            items:3, // from this breakpoint 960 to 1199
            margin:15, // and so on...
            center:false, 

          },

          1200:{

            items:3,
            margin: 25,

          }
        } 
      });
    }

  /*-------------------------------------
   Logo Slider jQuery activation code
   -------------------------------------*/

    $("#logo-slider").owlCarousel({
        // Most important owl features
        items : 5,  
        nav: true,
        navText: false,  
        dots: false,
        loop: true,
        autoplay: true,

        // Responsive options
        responsive: true,
        responsive:{
        0:{
          items:1, // In this configuration 1 is enabled from 0px up to 479px screen size
          centerMode:true,
        },

        480:{

          items:3, // from 480 to 677 
          nav:true, // from 480 to max 
          centerMode:true,

        },

        678:{

          items:4, // from this breakpoint 678 to 959
          centerMode:true, // only within 678 and next - 959
        },

        960:{

          items:5, // from this breakpoint 960 to 1199
          margin:20, // and so on...
          center:false, 

        },

        1200:{

          items:5,
          margin: 40,

        }
      } 
    });

    /*----------------------------
    single-productjs active
    ------------------------------ */

     $('.single-product').slick({
       slidesToShow: 1,
       slidesToScroll: 1,
       arrows: false,
       fade: true,
       asNavFor: '.single-product-nav'
     });
     $('.single-product-nav').slick({
       slidesToShow: 3,
       slidesToScroll: 1,
       asNavFor: '.single-product',
       dots: false,
       focusOnSelect: true,
       centerMode:true,
     });


 /*-------------------------------
    isotope menu sticky
    ---------------------------------*/  
    /* isotope Menu jquery isotope */
    var $container = $('#posts').isotope({
      itemSelector : '.item',
      isFitWidth: true
    });

      $container.isotope({
        columnWidth: '.col-sm-6'
      });
    
    $container.isotope({ filter: '.lunch' });

      // filter items on button click
    $('#filters').on( 'click', 'button', function() {
      var filterValue = $(this).attr('data-filter');
      $container.isotope({ filter: filterValue });
    });
    

/*----------------------------
    wow js active
    ------------------------------ */
    new WOW().init();

    // image loaded portfolio init
    $('.grid').imagesLoaded(function() {
        $('.portfolio-filter').on('click', 'button', function() {
            var filterValue = $(this).attr('data-filter');
            $grid.isotope({
                filter: filterValue
            });
        });
        var $grid = $('.grid').isotope({
            itemSelector: '.grid-item',
            percentPosition: true,
            masonry: {
                columnWidth: '.grid-item',
            }
        });
    });        

    // magnificPopup init
    $('.image-popup').magnificPopup({
        type: 'image',
        callbacks: {
            beforeOpen: function() {
               this.st.image.markup = this.st.image.markup.replace('mfp-figure', 'mfp-figure animated zoomInDown');
            }
        },
        gallery: {
            enabled: true
        }
    });
    
	//preloader
	$(window).load(function() {
		$("#loading").delay(2000).fadeOut(500);
		$("#loading-center").click(function() {
		$("#loading").fadeOut(500);
		})

    if($(window).width() < 992) {
      $('.rs-menu').css('height', '0');
      $('.rs-menu').css('opacity', '0');
      $('.rs-menu').css('z-index', '-1');
      $('.rs-menu-toggle').on( 'click', function(){
         $('.rs-menu').css('opacity', '1');
         $('.rs-menu').css('z-index', '1');
     });
    }

	})


 /*-------------------------------
    Counter Up
    ---------------------------------*/       
    var counter = $('.about-counter');
    if(counter.length) {   
      counter.counterUp({
        delay: 50,
        time: 3000
      });
    }

    // Get a quote popup

    $('.popup-quote').magnificPopup({
        type: 'inline',
        preloader: false,
        focus: '#qname',
        removalDelay: 500, //delay removal by X to allow out-animation
        // When elemened is focused, some mobile browsers in some cases zoom in
        // It looks not nice, so we disable it:
        callbacks: {
            beforeOpen: function() {
                this.st.mainClass = this.st.el.attr('data-effect');
                if($(window).width() < 700) {
                    this.st.focus = false;
                } else {
                    this.st.focus = '#qname';
                }
            }
        }
    });


    /*-------------------------------------
       Chefs Slider jQuery activation code
       -------------------------------------*/
    $("#owl-Chefs").owlCarousel({
        // Most important owl features
        items : 1,     
        // Navigation 
        nav: false,
        dotsText: ["<i class='fa fa-angle-left'></i>", "<i class='fa fa-angle-right'></i>"],
        dots: true,
    });


    /*-------------------------------------
       Testimonial Slider Two jQuery activation code
       -------------------------------------*/
    $("#testimonal-two").owlCarousel({
        // Most important owl features
        items : 1,     
        // Navigation 
        nav: false,
        dots: true,
    });



    /*-------------------------------------
       Testimonial Slider Two jQuery activation code
       -------------------------------------*/
    $("#whats-new-slider").owlCarousel({
        // Most important owl features
        items : 1,     
        // Navigation 
        nav: false,
        dots: false,
        loop:true,
        autoplay:true,
    });

    /*-------------------------------------
       Event Slick Slider jQuery activation code
       -------------------------------------*/

       $('.event-slider').slick({
      centerMode: true,
      centerPadding: '0',
      slidesToShow: 3,
      arrows: false,
      dots: true,
      responsive: [
        {
          breakpoint: 768,
          settings: {
            arrows: false,
            centerMode: true,
            centerPadding: '0',
            slidesToShow: 2
          }
        },
        {
          breakpoint: 480,
          settings: {
            arrows: false,
            centerMode: true,
            centerPadding: '0',
            slidesToShow: 1
          }
        }
      ]
    });

    /*-------------------------------------
     jQuery Main Menu activation code
     --------------------------------------*/

    $('.menu-item-has-children a').on("click", function(event) {
        event.preventDefault();
        var location = $(this).attr('href');
        window.location.href = location;
        return false;
    });
    /*-------------------------------------
    Main Menu jQuery activation code
    -------------------------------------*/
   $(".rs-menu ul li a")
        .on("click", function(e) {
            var link = $(this);

            var item = link.parent("li");
            
            if (item.hasClass("active")) {
                item.removeClass("active").children("a").removeClass("active");
            } else {
                item.addClass("active").children("a").addClass("active");
            }

            if (item.children("ul").length > 0) {
                var href = link.attr("href");
                link.attr("href", "#");
                setTimeout(function () { 
                    link.attr("href", href);
                }, 300);
                e.preventDefault();
            }
        })
        .each(function() {
            var link = $(this);
            if (link.get(0).href === location.href) {
                link.addClass("active").parents("li").addClass("active");
                return false;
            }
    });

 /*-------------------------------
    Our Menu
    ---------------------------------*/
    $('#filters button', this).on('click', function() {
        $('.btn').removeClass('active');
         $(this).addClass('active');
    });

    /*-------------------------------
    Main menu sticky
    ---------------------------------*/   

    var num = $('.header-area').innerHeight();
    var menu_height = $('.header-bottom-area').innerHeight();
    $(window).bind('scroll', function () {    
     if ($(window).scrollTop() >= num+menu_height) {
            $('.header-area').addClass('sticky-header');
      $('body').css({'padding-top':menu_height});
        } else {
            $('.header-area').removeClass('sticky-header');
      $('body').css({'padding-top':0});
        }        
    });

    /*--------------------------
     ScrollTop init Activation Code
    ---------------------------- */
    $(window).scroll(function() {
        if ($(this).scrollTop() >= 50) {        // If page is scrolled more than 50px
            $('#return-to-top').fadeIn(200);    // Fade in the arrow
        } else {
            $('#return-to-top').fadeOut(200);   // Else fade out the arrow
        }
    });
    $('#return-to-top').on('click', function() {      // When arrow is clicked
        $('body,html').animate({
            scrollTop : 0                       // Scroll to top of body
        }, 500);
    });

})(jQuery);