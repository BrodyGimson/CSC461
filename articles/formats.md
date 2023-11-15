---
layout: page
title: "Spherical Videos - Main Formats and the OMAF Standard"
---

There are two main formats to consider with spherical video which are monoscopic and stereoscopic. Both formats have higher bitrate requirements and lower latency requirements than standard video, due to the amount of data required to cover the full sphere and the user’s movement. Spherical videos are found in the same file formats, use the same encodings, and have the same delivery methods as standard videos. The data required to view them properly is stored in the metadata of the file, which is standardized by MPEG’s Omnidirectional Media Format (OMAF) standard.

### Monoscopic Videos
Monoscopic videos are the most straight-forward format. There is one video channel, so one spherical projection is used for both eyes. This format is commonly used for videos that won’t be viewed in an HMD (like a VR headset), such as on a phone or in a web browser. The bitrate is higher than standard videos, but is smaller than stereoscopic. When viewed in VR, these videos will have no depth and appear flat, offering very little immersion to the user.

To create a monoscopic 360 video, cameras simply require being able to capture all 360 degrees around them, which can be accomplished with as little as two fisheye lens cameras. This allows monoscopic cameras to be incredibly small, like the GoPro MAX [1]. After the footage has been captured, the videos need to be synced and stitched together, which will increase in complexity the more cameras there are.

### Stereoscopic Videos
This format is more complex as there are now two video channels, one for each eye. This adds depth to a video by mimicking how our eyes see depth by offseting the two channels. This format requires the use of an HMD to be viewed correctly, otherwise one channel can be viewed as monoscopic or both channels can be viewed side by side. Since there are two channels, stereoscopic requires a higher bitrate than monoscopic.

The process of creating a stereoscopic 360 video is similar to a monoscopic one, but with increased complexities and requirements. Camera’s now require lenses to be arranged in such a way that their viewpoints overlap, in order to capture both eyes' perspectives. When stitching the videos together, we now need to worry about not only syncing each camera, but making sure the two channels are set up correctly (i.e. the angle and distance looks correct while looking around). Since the user will be wearing a headset, any mistakes with this process will break the user's immersion. An example of a camera with this capability is the Insta360 Pro 2, which also does a lot of this complex stitching for you [2]. Stereoscopic capable cameras can also take monoscopic videos and tend to be more expensive than monoscopic cameras.

### The OMAF Standard
Created by the Motion Picture Experts Group (MPEG) as part of the MPEG-I standard (MPEG Immersive media) the OMAF standard was the first standardization of 360 videos, images, and audio. Its first version came out in the month of October in 2017 and had very basic support for this media [3]. It was superseded by version 2 in October 2020 which added support for overlays, multiple perspectives, and some basic support for 6DoF videos (explored further in the future work article). Both versions of OMAF support equirectangular and cubemap projections, although other projection types exist (explored further in the "Viewing" article).

## References
### Cited References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp;GoPro. “GoPro MAX 360 Action Camera.” GoPro.com. https://gopro.com/en/ca/shop/cameras/max/CHDHZ-202-master.html (accessed Nov. 15, 2023).
    </p>
    <p>
        [2]&nbsp;&nbsp;&nbsp;&nbsp;Insta360. “Insta360 Pro 2 - 360 VR Camera.” Insta360.com (accessed Nov. 15, 2023).
    </p>
    <p>
        [3]&nbsp;&nbsp;&nbsp;&nbsp;M. M. Hannuksela and Y. -K. Wang, "An Overview of Omnidirectional MediA Format (OMAF)," <em>Proceedings of the IEEE</em>, vol. 109, no. 9, pp. 1590-1606, Sept. 2021, doi: 10.1109/JPROC.2021.3063544.
    </p>
</div>

### General References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp;A. Yaqoob, T. Bi, and G. -M. Muntean, "A Survey on Adaptive 360° Video Streaming: Solutions, Challenges and Opportunities," <em>IEEE Communications Surveys & Tutorials</em>, vol. 22, no. 4, pp. 2801-2838, Jul. 2020, doi: 10.1109/COMST.2020.3006999.
    </p>
</div>

### Next Article - [Syncing and Stiching](/articles/syncing_and_stitching)