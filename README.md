# Segmented Video Compression
## myEncoder.py:
- This file breaks the video frames into foreground and background macroblocks with green representing the background and red the foreground. Then, the foreground and background are compressed using different quantization values. This results in the background (less important) being compressed more than the foreground. A resulting .cmp video files is created in the output folder.
## myDecoder.py:
- This file retrieves the .cmp file generated in our encoder and decodes the file using the corresponding n1 and n2 values.
## GUI.py:
- Creates a user interface that allows the user to watch the segmentation, compression, and decompression of the original video files. The user is able to play the entire result video synced up with the corresponding .wav file.
  
- To run this program, install all necessary imports
- Then, python3 GUI.py <input_video.rgb> <n1> <n2>
