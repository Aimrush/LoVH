# LoVH - A Multimodal Video Highlight Generation Framework for League of Legends

League of Video Highlights (LoVH), is an automatic video highlight generator for League of Legends based on a hybrid
event-based and excitement-based approach to dynamic summarization.
LoVH is a supervised learning framework comprised of an audio classifier for excitement detection and two image classifiers
for event classification and replay classification respectively.

---

## Code
In the near future.

---

## Dataset
Machine learning approaches to solve problems require a reliable dataset that reflects the real-world environment in 
which models can be trained and evaluated.

There are two images and one audio dataset presented:
- In-Game Notification Image Dataset
- Replay Image Dataset
- Audio Excitement Dataset

The two image datasets share a total of **40469** 1280 x 720 JPG files but contain individual label files.
The image labels of both datasets have been split into training, validation, and testing sets with a 60:20:20 ratio.
The audio dataset contains the label file of excited and unexcited audio segments with links to the full audio.

### 1. In-Game Notification Image Dataset
The "datasets/image/pop_frames_master.txt" file contains the labels of image frames that contain 
notification/popup message labeled as '1' or default '0'. It is randomly split into train, validate, and test sets.

The frames are named as "videoID_FrameNumber.jpg" e.g 1_148875.jpg -> video 1 and frame 148875 (Video ID's -> 
"datasets/video_list.txt")

To generate the frames download the videos in "datasets/video_list.txt" and run "video_to_img.ipynb" (use the labels
provided in place of the generated)

### 2. Replay Image Dataset
The "datasets/image/replay_frames_master.txt" file contains the labels of image frames that contain
replays labeled as '1' or default '0'. It is randomly split into train, validate, and test sets.

The frames are named as "videoID_FrameNumber.jpg" e.g 1_148875.jpg is video 1 and frame 148875 (Video ID's ->
"datasets/video_list.txt")

To generate the frames download the videos in "datasets/video_list.txt" and run "video_to_img.ipynb" (use the labels
provided in place of the generated) - **generate frames only once**

### 3. Audio
The "datasets/audio/audio_master.txt" file contains the labels of six matchs where '1' represents excited audio and '0'
unexcited audio.

Note: Extract audio (.wav) from the downloaded videos -> "video_to_audio.ipynb".

[//]: # (A sample dataset is provided here.)

[//]: # (Contact the [author]&#40;mailto:akhilesh.shiuram@gmail.com&#41; for the full dataset.)