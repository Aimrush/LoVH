# LoVH - A Multimodal Video Highlight Generation Framework for League of Legends

League of Video Highlights (LoVH), is an automatic video highlight generator for League of Legends based on a hybrid
event-based and excitement-based approach to dynamic summarization.
LoVH is a supervised learning framework comprised of an audio classifier for excitement detection and two image classifiers
for event classification and replay classification respectively.

---

## Code
Coming soon.

---

## Dataset
Machine learning approaches to solve problems require a reliable dataset that reflects the real-world environment in which models can be trained and evaluated.

There are two images and one audio dataset presented:
- In-Game Notification Image Dataset
- Replay Image Dataset
- Audio Excitement Dataset

The two image datasets share a total of **40469** 1280 x 720 JPG files but contain individual label files.
The image labels of both datasets have been split into training, validation, and testing sets with a 60:20:20 ratio.
The audio dataset contains the label file of excited and unexcited audio segments with links to the full audio.

A sample dataset is provided here.

Contact the [author](mailto:akhilesh.shiuram@gmail.com) for the full dataset.