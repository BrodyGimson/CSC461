---
layout: page
title: "Spherical Videos - Viewing"
---

As mentioned in the introduction, spherical videos follow the same file formats and encodings as standard videos, but have metadata that software uses to know how the video is to be played. One of the most important aspects is the type of projection the video is designed for. There are a number of different types of projections, but we will look at three of them which are equirectangular, cubemap, and pyramid.

### Equirectangular
This projection type is one of the OMAF supported types, and is likely one you have seen before without knowing. Most world maps use this type of projection in reverse to take our globe and show it on a flat surface. With equirectangular the projection works in the opposite way as if we were taking that flat world map (the video) and wrapping it in a sphere. Equirectangular is also considered to be viewport-independent, that is the whole 360 video is projected in uniform-quality. The main benefits of equirectangular projections is its simplicity since the video can be one image. The main drawbacks of equirectangular is the distortion and redundancy it introduces near the poles of the video. Think back to our world map example, where countries closer to the equator are better represented than countries that aren’t (like Russia and Canada). This distortion at the poles causes more pixels to be used in those areas, creating redundancy. Due to this redundancy, equirectangular projections tend to require higher bitrates than other types to achieve the same quality. Google has an article which includes some great diagrams of how this projections works [1].

### Cubemap
Like equirectangular, cubemap is supported by OMAF and is viewport-independent. The 360 video is broken into 6 sides of a cube and those sides are projected into the sphere. There is still some redundancy and distortion around the sides of the cube edges, but nowhere near the level found in equirectangular’s poles. Due to this, cubemap projections of the same quality as an equirectangular projection will use a lower bitrate. There is a little more complexity with cubemaps, requiring videos to be split and processed a bit more during projection, but the benefits are worth it. There are improvements to this projection such as Google’s proposed equi-angular cubemap projection which aims to remove more of that distortion around the edges of the cube sides [1]. You can find more details and projection diagrams in that article.

### Pyramid
Pyramid projection is not supported by OMAF at the moment and is considered a viewport-dependent projection. This means that a portion of the video will have much higher quality than other parts. This is often used if there is only action happening in front of the user, for example in a video taken from the cockpit of a plane we may not care about the wall behind us since it isn’t particularly interesting. This allows videos to use an even lower bitrate, at the expense of making part of the video’s quality much poorer. Meta's article on this projection offers some more insight and diagrams on how it works [2].


## References
### Cited References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp;C. Brown. "Bringing pixels front and center in VR video." Google - The Keyword. https://blog.google/products/google-ar-vr/bringing-pixels-front-and-center-vr-video/ (accessed: Nov. 6, 2023).
    </p>
    <p>
        [2]&nbsp;&nbsp;&nbsp;&nbsp;E. Kuzyakov and D. Pio. "Next-generation video encoding techniques for 360 video and VR" Engineering at Meta. https://engineering.fb.com/2016/01/21/virtual-reality/next-generation-video-encoding-techniques-for-360-video-and-vr/ (accessed: Nov. 6, 2023).
    </p>
</div>

### General References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp;A. Yaqoob, T. Bi, and G. -M. Muntean, "A Survey on Adaptive 360° Video Streaming: Solutions, Challenges and Opportunities," <em>IEEE Communications Surveys & Tutorials</em>, vol. 22, no. 4, pp. 2801-2838, Jul. 2020, doi: 10.1109/COMST.2020.3006999.
    </p>
    <p>
        [2]&nbsp;&nbsp;&nbsp;&nbsp;M. M. Hannuksela and Y. -K. Wang, "An Overview of Omnidirectional MediA Format (OMAF)," <em>Proceedings of the IEEE</em>, vol. 109, no. 9, pp. 1590-1606, Sept. 2021, doi: 10.1109/JPROC.2021.3063544.
    </p>
</div>

### Next Article - [Metadata Required for YouTube](/articles/metadata)