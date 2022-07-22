# Stop Motion Film Maker
This project consists of using opencvs in order to take picture frames and turn them into a fun stop motion film. 

| **Engineer** | **School** | **Area of Interest** | **Grade** |
|:--:|:--:|:--:|:--:|
| Esther Kpapu | Central Park East High School | Human Biology/biomechanical engineering | Incoming Senior

![Headstone Image](https://github.com/BlueStampEng/BSE_Template_Portfolio/blob/4655d8c4b2f1d0fa5912511d0b39542520b9f88e/branding/BlueStamp-Engineering-Logo-White.png) 

# Software code used:
-OpenCv-python 3.10(64 bits)

# Code 

```py
import cv2
 initialize the video stream
video_cap = cv2.VideoCapture(0)

 grab the width, height, and fps of the frames in the video stream.
frame_width = int(video_cap.get(cv2.CAP_PROP_FRAME_WIDTH))
frame_height = int(video_cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
fps = int(video_cap.get(cv2.CAP_PROP_FPS))

initialize the FourCC and a video writer object
fourcc = cv2.VideoWriter_fourcc(*'XVID')
output = cv2.VideoWriter('output.mp4', fourcc, fps, (frame_width, frame_height))

while True:
    success, frame = video_cap.read()
    cv2.imshow("frame", frame)
    # write the frame to the output file
    output.write(frame)
    if cv2.waitKey(20) == ord('q'):
        break
```

# Final Milestone

My final milestone is the demonstration step by step of how the code scripted actually works. My final milestone was a continuation of what I talked about in my fist milestone, as seen in this video I took a frame of whtatever object I want and it saved onto my file on my desktop tilted SCR. This is the position I want my whole project to be at, but thats not all to it. After taking the frame I want I would save it onto my computer with the other frames I want to work with and put all those together to create the "stop motion" effect I need. I also reliazed at the end that I can't take multiple shots at once so I had to do it all one at a time. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/Tl0eXKZv4QI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# First Milestone
  
My first milestone was setting up a code sequence for the base of my project. I first had to download python 3.10(64 bit) onto my windows laptop to be able to use the scrip type on my laptop. After downloading python I had to also download Visual Studio Code and OpenCvs as a way to enbale the code script to run properly. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/R3KhEzNtbq8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>{:target="_blank" rel="noopener"}
