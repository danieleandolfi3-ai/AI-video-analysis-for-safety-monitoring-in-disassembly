# AI-video-analysis-for-safety-monitoring-in-disassembly
The EasyMocap library is used to analyze videos of an operator performing pick-and-place and screwdriving tasks during the disassembly of an Electronic Pneumatic Module. The videos are recorded using RGB cameras in the Politecnico di Milano laboratory. This analysis makes it possible to identify and monitor potentially dangerous hand positions.

**Code explanation**

Three notebooks have been provided, each corresponding to an experiment described in the report. The code in each notebook is divided into three sections: Installation, Calibration Video Manipulation, and 3D KeyPoints Estimation. All the code can be executed on Google Colab.

**Installation**

The Installation section contains the necessary commands to install the required dependencies and functions needed for the subsequent sections.

**Calibration**

The Calibration section executes all the steps explained in the report. At the end of this process, the following folders contain the results:

**Extrinsic Parameters**

·Extri_data/videos  – contains the input calibration videos of each camera.

* Extri_data_2/images  – Contains selected frames for each camera.
* Extri_data_2/output/calibration  – Stores frames where the detected chessboard is present for each camera.
* Extri_data_2/chessboard  – Includes JSON files with 3D and 2D keypoint data.

**Intrinsic Parameters**

·Intri_data/videos  – contains the input calibration videos of each camera.

* Intri_data_2/images  – Contains selected frames for each camera.
* Intri_data_2/output/calibration  – Stores frames where the detected chessboard is present for each camera.
* Intri_data_2/chessboard  – Includes JSON files with 3D and 2D keypoint data.

**3D Points Estimation**

The 3D Points Estimation section executes all the steps described in the report. Upon completion, the results are stored in the following folders:

* task_data/annots  – Contains JSON files with 2D keypoints of both hands for each camera.
* task_data/images  – Stores frames extracted from the videos for each camera.
* task_data/keypoints3D/detect  – Stores frames extracted from the videos, highlighting the detected 2D keypoints.
* task_data/keypoints3D/keypoints2D  – Contains JSON files with 2D keypoints of both hands for each camera.
* task_data/keypoints3D/keypoints3D  – Contains JSON files with 3D keypoints of both hands.
* task_data/match  – Stores frames extracted from the videos, highlighting the detected 3D keypoints.
* task_data/match.mp4  – Provides the output video where 3D keypoints are highlighted.
* task_data/videos  – contains the input task videos of each camera.
* task_data/extri .yml – contains the extrinsic parameters of each camera.
* task_data/intri .yml – contains the intrinsic parameters of each camera
