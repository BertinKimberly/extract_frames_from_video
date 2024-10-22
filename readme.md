## Automatic Number Plate Recognition (ANPR) Dataset Creation

This project involves creating a dataset for an Automatic Number Plate Recognition (ANPR) system using raw video footage. The goal was to extract frames where vehicle number plates are clearly visible, and organize them into a structured dataset.


## Tools and Methods Used
'OpenCV': Used for automating the frame extraction process from the video footage. Frames were generated programmatically using OpenCV's video processing capabilities.
Manual Arrangement: After extracting the frames, they were manually reviewed to ensure the number plates were clearly visible. The frames were then organized in a structured format.
### Folder Structure
The dataset is structured as follows:

```bash
dataset/
│
├── car_1/
│   ├── frame_0000.jpg
│   ├── frame_0001.jpg
│   ├── ...
│   └── frame_0009.jpg
│
├── car_2/
│   ├── frame_0000.jpg
│   ├── frame_0001.jpg
│   ├── ...
│   └── frame_0009.jpg
│
└── 
```

Each folder represents a different vehicle, with car_1, car_2, etc., being unique identifiers for each car. Inside each folder, there are exactly 10 frames (frame_0000.jpg to frame_0009.jpg) where the number plates are clearly visible.

#### Steps to Complete the Task
Video Footage Review:

The video footage was carefully reviewed to identify frames where vehicle number plates were clearly visible.
##### Frame Extraction with OpenCV:

OpenCV was used to automate the extraction of frames from the video. A Python script was implemented to capture frames at intervals where the number plate was visible.
Manual Selection and Arrangement:

The extracted frames were reviewed, and only those with clearly visible number plates were selected.
The selected frames were then manually organized into folders based on the corresponding car.

### Challenges Faced
#### Frame Quality Variability:
Some frames had motion blur or poor lighting, making the number plates hard to read. These frames were discarded, and additional frames were extracted to ensure quality.
#### Automating Frame Selection:
Automating the identification of frames where number plates were visible required manual intervention, as the number plates were not consistently detectable using OpenCV's automated methods.
#### Experience Summary
This task provided hands-on experience with video processing using OpenCV and manual data curation. It highlighted the challenges of working with real-world data, particularly in ensuring the clarity of frames for ANPR applications.

### How to Use the Dataset
 Clone this repository:

```bash
git clone https://github.com/BertinKimberly/extract_frames_from_video.git
Navigate to the dataset directory to access the organized frames.
```