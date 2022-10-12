Use [OpenVINO toolkit](https://github.com/openvinotoolkit)

Image classification
- Created a HuggingFace Spaces to call OpenVINO model for inference (https://huggingface.co/spaces/rbarman/openvino_image_classification)
- Based on notebook: https://github.com/openvinotoolkit/openvino_notebooks/tree/main/notebooks/001-hello-world/
- Sent clue image to the HuggingFace spaces, but the recommended class does not seem useful or accurate. The Space currently uses MobileNet based model; might need to upgrade to something like Resnet50


Text Detection
- Created a HuggingFace Spaces to call OpenVINO model for inference (https://huggingface.co/spaces/rbarman/Openvino_Text_Detection)
- Based on notebook: https://github.com/openvinotoolkit/openvino_notebooks/tree/main/notebooks/004-hello-detection
- Sent clue image to HuggingFace spaces, but only detects highest word.
	- Added threshold adjustments
	- May need to try different model?