---
layout: post
category: deliverables
---
## Progress so Far
In regards to my bi-weekly schedule things are progressing nicely. I have an outline of what I want to discuss in the report and came up with a plan for what I want to demo.

During my research I have found that spherical videos are built on top of standard video file formats and codecs. All the info for how they are viewed is stored in the videos metadata which is standardized by the Omnidirectional Media Format (OMAF) from MPEG. The area during my readings that turned out to be the most interesting was the different types of video projections. Research into new projection types is ongoing, including work done by Meta [1] and Google [2].

The report I plan on breaking down into the following areas:
- Formats and MPEG's OMAF Standard
    - This section will introduce the different types of spherical videos and the devices they are designed to be viewed with
        - I.e. Monoscopic vs Stereoscopic
    - Will also introduce the OMAF standard, and the difference between the two versions
        - V1 vs V2
- Syncing and Stitching
    - This section will introduce the hardware these videos are filmed with and the software used to create them
        - Comparing complexity and pricing for each of the formats mentioned in the "Formats" section
- How these videos are viewed
    - This section will cover some spherical projection types
        - E.g. Equirectanguler, Cubemap, Meta's Pyramid, Google's Equi-Angular Cubemap
    - This will likely be the area with the most info and where my demo focuses
        - See "Technical Challenges" for more details on the demo
- Metadata needed for uploading to YouTube
    - My project proposal wanted to limit focus to what YouTube allows for spherical videos in this section
        - To bring an example in and limit the scope
    - This section will go over Google's requirements as that is what is used when uploading to YouTube [3]
        - V1 vs V2
        - Tools like Adobe Premiere have the ability to inject this metadata for you, but Google also provides a Python based injection tool that can be used [4]
- Interesting future work
    - 6DoF (Degrees of Freedom) filming
        - Videos that a user can look and walk around in

I explain my plans for the demo in the "Technical Challenges" section.

## Technical Challenges
### Challenges Met
Initially I was hoping to create my own spherical video as part of my demo, but it proved too challenging to get my hands on a camera that was capable of capturing one. This required me to rethink what I would demo, but the solution I came up with I believe will be more interesting to examine in the end.

### Challenges Solved
The solution I came up with was based off a suggestion from one of the TAs, which was to use a sample video from a sample dataset [5]. What I plan to do is use a conversion tool created by Samsung to convert it to different projection formats and qualtatively compare them (i.e. look at info redundancy and quality in the different formats) [6].

### Challenges Remaining
The last challenges will be to work with this Samsung tool to have a few videos of different formats and find a way to view the videos in the spherical and regular video modes to compare them. So far the multimedia program VLC seems to do well at viewing the equirectangular projection type, but not others [7]. Their beta version 4 may offer the ability to view other types, however it may be unstable or not work at all [8]. Viewing the videos in a flat format may be enough to compare them though and collect the data I need (i.e. screenshots to show in the demo and report). 


## What's Next
Next up will be to start making the report draft from the outline I have made and to tackle the last remaining technical challenges. Along with those I will need to create a presentaiton for the video demo and figure out what the best option will be to showcase the video on this site (i.e. an embeded unlisted YouTube video or if I can host it here).

One of the other things I want to do is to move my current research onto the website. I would create pages/articles that would cover the different aspects listed in my report that give a brief overview of each part (including some pictures and videos) which would be expanded upon in the actual report. My original impression was that the websites were just an area to post updates and the deliverables, so perhaps this could be clarified if these articles are expected or not.


## References
### Cited References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp; E. Kuzyakov and D. Pio. "Next-generation video encoding techniques for 360 video and VR" Engineering at Meta. https://engineering.fb.com/2016/01/21/virtual-reality/next-generation-video-encoding-techniques-for-360-video-and-vr/ (accessed: Nov. 6, 2023).
    </p>
    <p>
        [2]&nbsp;&nbsp;&nbsp;&nbsp; C. Brown. "Bringing pixels front and center in VR video." Google - The Keyword. https://blog.google/products/google-ar-vr/bringing-pixels-front-and-center-vr-video/ (accessed: Nov. 6, 2023).
    </p>
    <p>
        [3]&nbsp;&nbsp;&nbsp;&nbsp; *Spatial Media*. (2018), Google. Accessed: Nov. 6, 2023. [Source Code]. Available: https://github.com/google/spatial-media/tree/v2.1
    </p>
    <p>
        [4]&nbsp;&nbsp;&nbsp;&nbsp; Google. "Upload 180- or 360-degree videos." Youtube Help. https://support.google.com/youtube/answer/6178631 (accessed: Nov. 6, 2023).
    </p>
    <p>
        [5]&nbsp;&nbsp;&nbsp;&nbsp; *A-large-dataset-of-360-video-user-behaviour*. (2021), 360VidStr. Accessed: Nov. 6, 2023. [Source Code]. Available: https://github.com/360VidStr/A-large-dataset-of-360-video-user-behaviour/tree/main
    </p>
    <p>
        [6]&nbsp;&nbsp;&nbsp;&nbsp; *360tools*. (2016), Samsung. Accessed: Nov. 6, 2023. [Source Code]. Available: https://github.com/Samsung/360tools
    </p>
    <p>
        [7]&nbsp;&nbsp;&nbsp;&nbsp; VideoLAN. "360° Video playback with VLC." VLS User Documentation. https://docs.videolan.me/vlc-user/3.0/en/advanced/player/360_video.html (accessed: Nov. 6, 2023).
    </p>
    <p>
        [8]&nbsp;&nbsp;&nbsp;&nbsp; VideoLan. "VLC media player nightly builds." VideoLAN Organization. https://nightlies.videolan.org/ (accessed: Nov. 6, 2023).
    </p>
</div>

### General References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp; A. Yaqoob, T. Bi, and G. -M. Muntean, "A Survey on Adaptive 360° Video Streaming: Solutions, Challenges and Opportunities," *IEEE Communications Surveys & Tutorials*, vol. 22, no. 4, pp. 2801-2838, Jul. 2020, doi: 10.1109/COMST.2020.3006999.
    </p>
    <p>
        [2]&nbsp;&nbsp;&nbsp;&nbsp; M. M. Hannuksela, Y. -K. Wang and A. Hourunranta, "An Overview of the OMAF Standard for 360° Video," *2019 Data Compression Conference (DCC)*, Snowbird, UT, USA, 2019, pp. 418-427, doi: 10.1109/DCC.2019.00050.
    </p>
    <p>
        [3]&nbsp;&nbsp;&nbsp;&nbsp; M. M. Hannuksela and Y. -K. Wang, "An Overview of Omnidirectional MediA Format (OMAF)," *Proceedings of the IEEE*, vol. 109, no. 9, pp. 1590-1606, Sept. 2021, doi: 10.1109/JPROC.2021.3063544.
    </p>
</div>