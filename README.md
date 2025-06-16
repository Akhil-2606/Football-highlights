# Football-highlights
This project consists of two Python scripts that utilize computer vision and media processing to **automatically detect hand gestures from videos** and **generate highlight reels** based on in-game events.

# Overview
The system is designed to:
1. Detect specific hand gestures from a video (Index Finger, V Sign, Little Finger).
2. Log each detected gesture with a timestamp and associated team score.
3. Create a highlight video showcasing moments when gestures were detected.

# Features 
1.Gesture Detection with OpenCV and MediaPipe
The system watches the video and recognizes specific hand gestures.

Each gesture means either a team scored or a highlight should be marked.

2.Highlight Video Creation with Overlays
It cuts short clips from the video where gestures were found.

Adds team names, scores, and time on the screen to make it easy to follow.

3.Slow Motion and Visual Effects
Can show important moments in slow motion.

Adds clear text and background colors to highlight what’s happening.

4.CSV and Video Output
Saves all gesture times and scores in a CSV file.

Creates a final highlight video that can be easily shared.
# Setup 
Step 1: Detect Gestures and Generate Scores 

python Computer_vision.py

Ensure the video filename is set correctly inside the script (e.g., VideoA.mp4).

Step 2: Generate Highlights from CSV

python Highlights1.py

Make sure to update the csv_files list with your .csv files:

csv_files = ['VideoA_scores.csv']

# Output
VideoA_scores.csv – Log of score and gesture events.

VideoA_highlights.mp4 – Automatically generated highlight reel.


