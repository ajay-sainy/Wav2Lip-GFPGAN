<h1 align="center">wav2lip (High Definition)<br><sup><sub>Alternative to Flawless AI's TrueSync<br>  <sup>Run the code on &nbsp;</sup><a target="_blank" href="https://colab.research.google.com/github/indianajson/wav2lip-HD/blob/main/colab.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg"/></a> &nbsp; 
  </sub></sup>
 </h1>

### What is this?

An advanced lip syncing software, allowing you to change the lip movements in a high resolution video file to match a provided voice from an audio file. This repository contains the code to easily perform the synchronization using the power of Wav2Lip and GFPGAN. This software can be used to make film dubbing more effective, by syncing the lip movement of the actors to the new dubbed audio. 

### Usage

1. Visit [this link](https://colab.research.google.com/github/indianajson/wav2lip-HD/blob/main/colab.ipynb) to launch the program in Google Colab.
2. Run the first code block labeled "Installation". This will take 1-2 minutes.
3. Upload a video file and audio file to the `wav2lip-HD/inputs` folder in Colab.
4. Change the file names in the block of code labeled `Synchronize Video and Speech` and run the code block. \
5. Once 

### Important Reminders

- The video file should contain only one face.
- Every frame of the video must contain the face. 
- The software will trim the video if audio ends first. To bypass, add a snippet of audio to that makes it longer than the video, then trim the video.
- You will need to combine the audio and video into a single file after processing. 

### Credits

Originally created by [@ajay-sainy](https://github.com/ajay-sainy/), this repository contains an updated Google Colab file for ease of use, as well as, an updated requirements.txt, which is necessary to run the code on today's version of Google Colab. 
