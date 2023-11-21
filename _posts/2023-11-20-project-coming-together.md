---
layout: post
---
The project is coming together nicely. As I mentioned in my midterm update I wanted to take some of the research I did and post it as articles on the site. So far I have finalized half of what I would like up, and have 2 drafts I am still working on. These not only have helped summarize what I have learned so far, but are helping me create a report draft as well. I plan to finish up the last articles and have them posted soon which will work well with my hope to have a report draft ready in the next 2 weeks.

For the demo I ran into a bit of a snag but was able to overcome it. My original plan of using Samsung’s 360tools [1] didn’t turn out well, as the tool didn’t work as I had hoped. It required files to be in a particular format and would only convert a few frames of the video, not the whole thing. This required me to take a step back and think of an alternative tool to do what I originally wanted, otherwise I could really only compare stills of the video. 

I ended up finding out the well known tool FFmpeg has a filter designed for converting 360 video projection formats called v360 [2]. I used this filter to create cubemap and truncated square pyramid projection versions of one of the videos from the sample video dataset [3]. They turned out really well and can be viewed in flat format using FFplay which is included with FFmpeg. I want to see if I can get them viewed in spherical format as well, but the flat format will suffice for comparison if I cannot. I have found a tool by Nokia designed for testing out features of the OMAF standard that looks promising and I plan to see if it will work for the demo [4].

## References
<div style="text-indent: -36px; padding-left: 36px;">
    <p>
        [1]&nbsp;&nbsp;&nbsp;&nbsp;<em>360tools</em>. (2016), Samsung. Accessed: Nov. 20, 2023. [Source Code]. Available: https://github.com/Samsung/360tools
    </p>
    <p>
        [2]&nbsp;&nbsp;&nbsp;&nbsp;<em>FFmpeg</em>. (v6.1), FFmpeg. Accessed: Nov. 20, 2023. [Online]. Available: https://www.ffmpeg.org/
    </p>
    <p>
        [3]&nbsp;&nbsp;&nbsp;&nbsp;<em>A-large-dataset-of-360-video-user-behaviour</em>. (2021), 360VidStr. Accessed: Nov. 6, 2023. [Source Code]. Available: https://github.com/360VidStr/A-large-dataset-of-360-video-user-behaviour/tree/main
    </p>
    <p>
        [4]&nbsp;&nbsp;&nbsp;&nbsp;<em>OMAF</em>. (v2.0.0), Nokia. Accessed: Nov. 20, 2023. [Source Code]. Available: https://github.com/nokiatech/omaf
    </p>
</div>