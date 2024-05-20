# TSEC-Dataset
Traffic Scenarios Event Caption (TSEC) Dataset for training and testing video captioning methods for driving scenes
![Examples of TSEC dataset](Examples%20of%20the%20TSEC%20dataset.png)
# What is TSEC-Dataset
General video captioning datasets are not suitable for the characteristics of driving scenes. To address this issue, we develop the Traffic Scenarios Event Caption (TSEC) Dataset to describe the key events of ego vehicle, road environment and other traffic participants. To acquire diverse types of traffic scenarios, we select the
videos that we take with our on-board camera and other public dataset videos. We also download from BiliBili and Youtube to get the traffic accident videos. Because each video
of these may contain many traffic events, we spilt the videos into distinct clips and make each sub-clip associated with 1 to 3 key events.

We follow the rules when processing the video clips: 1) In order to increase the diversity, different weathers, different periods, different road conditions and different vehicle conditions need to be selected. 2) Due to the complexity of traffic situations at intersections, a number of intersection scenarios are chosen. 3) The clip needs to contain the entire event. 4) Discard clips that are difficult to judge. Based on the above principles, we obtain 8,000 video clips with a total duration of 11.5 hours.
# Annotation
During annotation, participants are told to imagine themselves as drivers to simulate the in-car experience. The videosshown to participants are raw videos without captions. We
randomize the order of sampled videos to reduce bias. Furthermore, considering the subjectivity in evaluating key events, weinitially use a voting method to label the types of key events in the current scene. Through this approach, we identify the top four key events with the highest number of votes for eachvideo, which are then detailed
