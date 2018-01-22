# Recommended video encoding settings
Below are recommended upload encoding settings for your videos.

### Container: MP4
  - No Edit Lists (or the video might not get processed correctly)
  - moov atom at the front of the file (Fast Start)

### Audio codec: AAC-LC
  - Channels: Stereo or Stereo + 5.1
  - Sample rate 96khz or 48khz

### Video codec: H.264
  - Progressive scan (no interlacing)
  - High Profile
  - 2 consecutive B frames
  - Closed GOP. GOP of half the frame rate.
  - CABAC Variable bitrate.
  - No bitrate limit required, though we offer recommended bit rates below for reference
  - Chroma subsampling: 4:2:0

### Frame rate
  - Content should be encoded and uploaded in the same frame rate it was recorded.
  - Common frame rates include: 24, 25, 30, 48, 50, 60 frames per second (other frame rates are also acceptable).
  - Interlaced content should be deinterlaced before uploading. For example, 1080i60 content should be deinterlaced to 1080p30, going from 60 interlaced fields per second to 30 progressive frames per second.

### Bitrate
The bitrates below are recommendations for uploads. Audio playback bitrate is not related to video resolution.
1/ Recommended video bitrates for SDR uploads
To view new 4K uploads in 4K, use a browser or device that supports VP9.

<img width="469" alt="screen shot 2018-01-15 at 11 35 42" src="https://user-images.githubusercontent.com/285033/34938335-4592831a-f9e8-11e7-80a8-1612aa462d2b.png">


2/ Recommended video bitrates for HDR uploads

<img width="466" alt="screen shot 2018-01-15 at 11 35 35" src="https://user-images.githubusercontent.com/285033/34938341-4acdfa26-f9e8-11e7-8617-2d7c7b0a8117.png">


3/ Recommended audio bitrates for uploads

<img width="167" alt="screen shot 2018-01-15 at 11 35 30" src="https://user-images.githubusercontent.com/285033/34938347-4fa0f1d4-f9e8-11e7-91be-38918de86428.png">


### Resolution and aspect ratio
We use 16:9 aspect ratio players. If you're uploading a non-16:9 file, it will be processed and displayed with either black bars on the left and right (pillar boxes) or black bars at the top and bottom (letterboxes) to make a 16:9 ratio in the player. 
