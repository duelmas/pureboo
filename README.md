# pureboo
A Pure HTML and Bootstrap approach to an image gallery.


Found this code a few years back in a random online forum somewhere...
<br><br>

I don't remember where that was but if anyone knows, I can give credit.
<br><br>
Anyhow, this is pure HTML with bootstrap.
<br><br>
It is a rather nice option for image galleries and viewing images online.
<br><br>
Carosels inside of modals oh my.
<br><br>
Click a thumbnail image, it will open modal and select image in the carosel that can match.
<br><br>
...and added controls to select to the next image.
<br><br>
Mockup for four images in this example.
<h2>Thumbmodosel [dot] HTML</h2>
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Bootstrap demo</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-4bw+/aepP/YC94hEpVNVgiZdgIC5+VKNBQNGCHeKRQN+PtmoHDEXuppvnDJzQIu9" crossorigin="anonymous">
  </head>
  <body>
    <!-- Modal Gallery -->

    <div class="modal fade" id="imgMoo" tabindex="-1" aria-labelledby="moody" aria-hidden="true">

      <div class="modal-dialog modal-fullscreen">
        <div class="modal-content">

          <div class="modal-header justify-content-center">
           <!-- Modal Header -->
           <h2 class="modal-title" id="moody">carosel in modal slide w thumbs</h2>
           <br>
      <br>
           <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>

          <div class="modal-body">

            <div id="image-slider" class="carousel slide" data-bs-ride="carousel">

          <div class="carousel-inner" aria-labelledby="moody">
            <div class="carousel-item active" data-bs-slide-to="0" data-bs-interval="false">
              <img src="image-1.jpg" alt="image 1">
              <h5>abstract 1</h5>
            </div>
            <div class="carousel-item" data-bs-slide-to="1" data-bs-interval="false">
              <img id="img2" style="display: inline-block" data-src="image-2.jpg" alt="image 2">
              <h5>abstract 2</h5>
            </div>
            <div class="carousel-item" data-bs-slide-to="2" data-bs-interval="false">
               <img id="img3" style="display: inline-block" data-src="image-3.jpg" alt="image 3">
               <h5>abstract 3</h5>
            </div>
            <div class="carousel-item" data-bs-slide-to="3" data-bs-interval="false">
                <img id="img4" style="display: inline-block" data-src="image-4.jpg" alt="image 4">
               <h5>abstract 4</h5>
            </div>
              </div>

              <!-- Carousel controls -->

            </div>

          </div>

          <div class="modal-footer" style="background:black;">
            <a class="btn btn-dark" href="#image-slider" data-bs-slide="prev">Prev</a>
            <a class="btn btn-dark" href="#image-slider" data-bs-slide="next">Next</a>
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>

          </div>

        </div>
      </div>

    </div>

    <div class="container">

      <div class="row">

        <div class="col">
          <a href="#image-slider" data-bs-slide-to="0">
            <img src="image-1-247x300.jpg" class="img-thumbnail img-fluid" data-bs-toggle="modal" data-bs-target="#imgMoo" alt="image 1">
          </a>
        </div>

        <div class="col">
           <a href="#image-slider" data-bs-slide-to="1">
             <img src="image-2-247x300.jpg" class="img-thumbnail img-fluid" data-bs-toggle="modal" data-bs-target="#imgMoo" alt="image 2">
           </a>
        </div>

        <div class="col">
           <a href="#image-slider" data-bs-slide-to="2">
             <img src="image-3-247x300.jpg" class="img-thumbnail img-fluid" data-bs-toggle="modal" data-bs-target="#imgMoo" alt="image 3">
           </a>
        </div>

        <div class="col">
           <a href="#image-slider" data-bs-slide-to="3">
             <img src="image-4-247x300.jpg" class="img-thumbnail img-fluid" data-bs-toggle="modal" data-bs-target="#imgMoo" alt="image 4">
           </a>
        </div>

        <!-- additional thumbnails here -->

      </div>

    </div>
    <!-- END MODAL AND thumbnails -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/js/bootstrap.bundle.min.js" integrity="sha384-HwwvtgBNo3bZJJLYd8oVXjrBZt8cqVSpeBNS5n7C8IVInixGAoxmnlMuBnhbgrkm" crossorigin="anonymous"></script>
  </body>
</html>

