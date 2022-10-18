Use [OpenVINO toolkit](https://github.com/openvinotoolkit)

Image Classification
- Created google colab notebook to call OpenVINO PaddlePaddle model for inference
- Based on notebooke: https://github.com/openvinotoolkit/openvino_notebooks/blob/main/notebooks/214-vision-paddle-classification/214-vision-paddle-classification.ipynb
- TODO: create hugging space with mutli label output.


Action recognition
- Created google colab notebook to call OpenVINO model for inference
- Based on notebook: https://github.com/openvinotoolkit/openvino_notebooks/tree/main/notebooks/403-action-recognition-webcam
- THe clue video was few seconds and seemed too short for the model to make an inference
- I duplicated the video several times to to make it longer ex:

```python
from moviepy.editor import VideoFileClip, concatenate_videoclips
clip_1 = VideoFileClip("clue.mp4")
clip_2 = VideoFileClip("clue.mp4")
final_clip = concatenate_videoclips([clip_1,clip_2])
final_clip.write_videofile("final.mp4")
```