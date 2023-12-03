---
layout: page
title: "Spherical Video - Metadata Required for YouTube"
---

An interesting area that shows a bit of history is looking at Google’s spherical media requirements for uploading to Youtube. There have been two versions, v1 which was released in 2015 before OMAF existed and v2 superseded it around 2016 when OMAF was being developed.

## V1 [1]
The original proposed scheme by Google used two types of metadata, global which was in the form of an XML file and local which was stored along with video frames. The global data contained information that pertained to the whole video such as the software used to stitch the video together and what type of projection is used in the video. In version 1 the only projection format that was supported was equirectangular, but it was designed to support more in the future if this scheme stuck around. The local data contained info such as GPS location of the shot.

## V2 [2]
Metadata in v2 is stored in four-character-code (4CC) boxes, which is the standard used by ISOBMFF (International Organization for Standardization Base Media File Format) files (MPEG-4) for metadata. The boxes are stored with the video tracks of the file, and start in the Spherical Video box (coded sv3d). This box then contains other boxes which will include info such as the projection type. This version, like OMAF, supports both equirectangular and cubemap projections. Google provides a tool to add their expected metadata in their Spatial Media tools [3], and some tools support adding the metadata themselves if you specify your plan on uploading the video to Youtube. It is also worth noting that videos can have v1 and v2 of this standard in the same file and they won’t conflict adding some backwards compatibility.

## Spatial Media vs OMAF Standard
Even though Google’s standard supports the same projections, it actually differs from OMAF.  Multiple video players support both this type of metadata and OMAF as they are relatively separate. For example Nokia has an OMAF video player and creator which supports both standards [4]. Google’s standard doesn’t support the same features of OMAF v2, such as overlay videos, but does have one thing over OMAF. The Spatial media standard supports not only MP4 but WebM as well. The metadata is stored differently between the two file types, but both are outlined. The format outlined in the article was for MP4, the WebM format can be explored further in Google’s repo if the reader is so inclined.

## References
### Cited References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp;<em>Spatial Media - Spherical Video RFC</em>. (2023), Google. Accessed: Dec. 3, 2023. [Source Code]. Available: https://github.com/google/spatial-media/blob/master/docs/spherical-video-rfc.md
    </p>
    <p>
        [2]&nbsp;&nbsp;&nbsp;&nbsp;<em>Spatial Media - Spherical Video V2 RFC</em>. (2020), Google. Accessed: Dec. 3, 2023. [Source Code]. Available: https://github.com/google/spatial-media/blob/master/docs/spherical-video-v2-rfc.md
    </p>
    <p>
        [3]&nbsp;&nbsp;&nbsp;&nbsp;<em>Spatial Media Metadata Injector</em>. (2023), Google. Accessed: Dec. 3, 2023. [Source Code]. Available: https://github.com/google/spatial-media/tree/master/spatialmedia
    </p>
    <p>
        [4]&nbsp;&nbsp;&nbsp;&nbsp;<em>OMAF</em>. (v2.0.0), Nokia. Accessed: Dec. 3, 2023. [Source Code]. Available: https://github.com/nokiatech/omaf
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

### Next Article - [Other Formats and Future Work](/CSC461/articles/future_work)