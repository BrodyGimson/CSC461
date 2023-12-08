---
layout: page
title: "Spherical Video - Syncing and Stiching"
---

The process of syncing and stitching is required to bring the multiple videos captured by the different camera lenses into one continuous spherical video. These multiple videos need to be synced in time and stitched together in order to create a seamless sphere. Stitching tends to be the area where most problems arise, where artifacts and seams can be seen if stitching is done poorly. It also should be noted that the more video channels we have in the video (ie.e stereoscopic vs monoscopic) and the more cameras we have the more syncing and stitching is required. A particular problem that arises with stereoscopic videos is making sure that the offset between the two channels is retained throughout the different views in the video, otherwise it can be very disorienting to the user. This can be tricky to view as one requires a headset to really see it properly.

Once a video is in a full sphere in our program, we can encode it into a spherical projection, and provide the metadata needed for the platform or software we wish to play it in. There are a few programs that offer this ability, including Adobe Premiere Pro [1], and some cameras even do it for you with varying levels of success, like Insta360’s Pro 2 which would be quite the task to handle manually [2]. Metadata can be added for you by these programs, or injected in post with tools like Google’s Python based Spatial Media Metadata Injector tool [3].

Here is a tutorial using Adobe After Effects which does a great job of showing how to manually sync and stitch a two lens monoscopic video for those wanting a more visual explanation: [https://www.youtube.com/watch?v=1idjcc2X_FU](https://www.youtube.com/watch?v=1idjcc2X_FU)

## References
### Cited References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp;Adobe. "Edit 360/VR Video." Creativecloud.Adobe.com. https://creativecloud.adobe.com/en-CA/learn/premiere-pro/web/edit-360-vr-video (accessed Dec. 8, 20-23).
    </p>
    <p>
        [2]&nbsp;&nbsp;&nbsp;&nbsp;Insta360. “Insta360 Pro 2 - 360 VR Camera.” Insta360.com. https://www.insta360.com/product/insta360-pro2 (accessed Nov. 15, 2023).
    </p>
    <p>
        [3]&nbsp;&nbsp;&nbsp;&nbsp;<em>Spatial Media Metadata Injector</em>. (2023), Google. Accessed: Dec. 3, 2023. [Source Code]. Available: https://github.com/google/spatial-media/tree/master/spatialmedia
    </p>
</div>

### General References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp;A. Yaqoob, T. Bi, and G. -M. Muntean, "A Survey on Adaptive 360° Video Streaming: Solutions, Challenges and Opportunities," <em>IEEE Communications Surveys & Tutorials</em>, vol. 22, no. 4, pp. 2801-2838, Jul. 2020, doi: 10.1109/COMST.2020.3006999.
    </p>
</div>

### Next Article - [Viewing](/CSC461/articles/viewing)