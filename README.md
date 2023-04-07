<h1 align="center">wav2lip (High Definition)<br><sup><sub>Alternative to Flawless AI's TrueSync<br>  <sup>Run the code on &nbsp;</sup><a target="_blank" href="https://colab.research.google.com/github/indianajson/wav2lip-HD/blob/main/colab.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg"/></a> &nbsp; 
  </sub></sup>
 </h1>

An advanced lip syncing software, allowing you to change the lip movements in a high resolution video file to match a provided voice from an audio file. This repository contains the code to easily perform the synchronization using the power of Wav2Lip and GFPGAN on Google Colaboratory. 

### How to Use

1. Visit [this link](https://colab.research.google.com/github/indianajson/wav2lip-HD/blob/main/colab.ipynb) to launch the program in Google Colab.
2. Run the first code block labeled "Installation". This will take 1-2 minutes.
3. Upload a video file and audio file to the `wav2lip-HD/inputs` folder in Colab.
4. Change the file names in the block of code labeled `Synchronize Video and Speech` and run the code block. 
5. Once finished run the code block labeled `Boost the Resolution` to increase the quality of the face.
6. Download your file from `wav2lip-HD/outputs` likely named `output_0000.mp4`.

### FAQs
 
1. There is some weird artifacting around the lips in my output. How do I fix this?

> If your output has odd lip shape or artifacts add the --nosmooth command to the `python inference.py` line in the second code block.

2. My video contains two speakers / pairs of lips, what do I do? 

> The video file should contain only one face. Simply mask out other faces before uploading your video file.

3. I got an error saying a face wasn't detected? What happened?

> Every frame of the video MUST contain the face or the program will crash. If every frame contains the face, it is possible the program is unable to see the face in certain frames. Try splitting your video and processing it in two parts to see where the issue exists. 

### Limitations

- The software will trim the video if audio ends first. To bypass, add a snippet of audio to that makes it longer than the video, then trim the video.
- You will need to combine the audio and video into a single file after processing. 
- The software cannot handle extreme poses or face positions.

### Ethical Use Cases

Software like this can be easily abused for unethical and immoral purposes, but there are several ethical use cases for this type of software. 

- *Creating High Quality Dubbings* - This software can be used to make film dubbing more effective, by syncing the lip movement of the actors to the new dubbed audio. 
- *Modifying Lines of Dialogue* - Directors may choose to modify a line of dialogue in post-production. With this software, the lips can be synced to the new audio without reshooting the scene.
- *Removing Expletives* - Directors may choose to remove some curse words for the sake of better film rating. With this software, the lips can be synced to the audio without the expletives, hiding the fact that it was removed. 

### Credits

Originally created by [@ajay-sainy](https://github.com/ajay-sainy/), this repository contains an updated Google Colab file for ease of use, as well as, an updated requirements.txt, which is necessary to run the code on today's version of Google Colab. 
