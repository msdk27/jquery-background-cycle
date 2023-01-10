# jquery-background-cycle

A Modified Version of Background Cycle jQuery plugin

Original plugin: https://www.jqueryscript.net/slideshow/Simple-jQuery-Background-Image-Slideshow-with-Fade-Transitions-Background-Cycle.html

The original plugin transition images automatically. I needed a plugin that changes image only when a button is clicked. This modified plugin serves that purpose.

Example Usage:

```
<script>
const bgCycle = $("body").backgroundCycle({
    imageUrls: [
        'img/photo-01.jpg',
        'img/photo-02.jpg',
        'img/photo-03.jpg',
        'img/photo-04.jpg',
        'img/photo-05.jpg'
    ],
    fadeSpeed: 2000,
    duration: -1,
    backgroundSize: SCALING_MODE_COVER
});

$('.link').click(function (e) {
    const previousImageId = 0;  // Change according to your needs
    const currentImageId = 1;   // Change according to your needs

    bgCycle.cycleToNextImage(previousImageId, currentImageId);
})
</script>
```
