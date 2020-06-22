1.Created a presentation webpage .
2.Overflow:HIDDEN to disable scroll bar.
3.Smooth scrolling added via jquery.
Smooth scroll jquery snippet
<script>
    $('.btn').on('click', function(event) {
        if (this.hash !== '') {
          event.preventDefault();
          const hash = this.hash;
          $('html, body').animate(
            {
              scrollTop: $(hash).offset().top
            },
            800
          );
        }
      });
  </script>
  jquery CDN:<script
  src="https://code.jquery.com/jquery-3.5.1.min.js"
  integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0="
  crossorigin="anonymous"></script>
  