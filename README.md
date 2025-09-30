# Awesome 3d Datasets

Last updated: <!--LAST_UPDATED--> 2025-09-30

## 🌟 Overview

- [Awesome 3d Datasets](#awesome-3d-datasets)
  - [🌟 Overview](#-overview)
  - [📄 Citation](#-citation)
  - [📚 3D Datasets Summary](#-3d-datasets-summary)
    - [👤 Human](#-human)
    - [🎯 Object](#-object)
    - [🏙️ Scene](#️-scene)
    - [📊 Modalities of 3D datasets](#-modalities-of-3d-datasets)
  - [⚒️ Applications](#️-applications)
    - [🔄 3D Reconstruct](#-3d-reconstruct)
    - [✨ 3D Generation](#-3d-generation)
    - [🎬 Video Generation](#-video-generation)
    - [🌐 World Models](#-world-models)

## 📄 Citation

> Coming soon

## 📚 3D Datasets Summary

### 👤 Human



| Dataset                                                                 | Year | Granularity | Tasks                                                                                           | Size  | Site                                                                                  | Description                                                                                                                                                                                                 |
|-------------------------------------------------------------------------|------|-------------|------------------------------------------------------------------------------------------------|-------|---------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [GigaHands](https://arxiv.org/abs/2412.04244)                           | 2025 | Human Hand  | 3D bimanual hand     | 14K   | [Github](https://github.com/Kristen-Z/GigaHands)                                      | A large dataset of bimanual hand–object interactions with 183 million frames, dense annotations (per hand & object), and 51 camera views for motion clips.                                                   |
| [H3WB](https://arxiv.org/pdf/2211.15692)                                | 2022 | Human Body  | 3D Pose Estimation     | 100K   | [Github](https://github.com/wholebody3d/wholebody3d)                                      | H3WB augments Human3.6M with 133 whole-body 3D keypoint annotations (body, hands, face, feet) for 100k images via a multi-view annotation pipeline.                                                   |
| [FaceScape](https://arxiv.org/pdf/2003.13989) | 2020 | Human Face  | Classification, Segmentation, Reconstruction, Completion, Recognition |  18K    | [Github](https://github.com/zhuhao-nju/facescape)    | 18,760 high-quality textured 3D face meshes from 938 people with pore-level geometry, uniform topology base meshes + displacement maps, and 20 expressions per subject

### 🎯 Object



| Dataset                                                      | Year | Granularity | Tasks                                                        | Size | Site                                                         | Description                 
| ------------------------------------------------------------ | ---- | ----------- | ------------------------------------------------------------ | ---- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [HPSketch](https://www.sciencedirect.com/science/article/abs/pii/S0010448525000107) | 2025 | Object | - | 151.9K  | [Github](-) | A history-based parametric CAD sketch dataset with advanced engineering commands; includes 151,984 sketches, 377,623 loops, and 29 command types for learning sketch histories and operations. |
| [CBF](https://arxiv.org/abs/2504.07378) | 2025 | Object | - | 20K  | [Github](-) | 20,000 CAD B-rep models composed of a base plate plus three geometric features each, with per-face labels stored in JSON; released with BRepFormer to benchmark complex geometric feature recognition on B-reps. |
| [Parametric 20000](https://data.mendeley.com/datasets/k6yzcks7g4/1) | 2024 | Object | - | 20K  | [Link](https://data.mendeley.com/datasets/k6yzcks7g4/1) | Multi-modal CAD shapes: each instance includes a point cloud, a triangle mesh, and a B-Rep file. |
| [WildRGB-D](https://arxiv.org/abs/2401.12592) | 2024 | Object | View Synthesis, Pose Estimation, 6D Object Tracking, 3D Reconstruction | 8.5K  | [Github](https://wildrgbd.github.io/) | A large-scale real-world RGB-D object video collection (~20K videos, 8.5K objects) with 360° views, diverse backgrounds, object masks, real-scale camera poses, and aggregated point clouds. |
| [BRep2Seq](https://academic.oup.com/jcde/article/11/1/110/7582276) | 2024 | Object | - | 1M  | [Link](-) | Introduces a synthetic CAD dataset (~1,000,000 models) of B-rep solids paired with feature-based construction sequences, and a hierarchical Transformer (Brep2Seq) for reconstructing/generating editable CAD models. |
| [Objaverse](https://arxiv.org/abs/2304.00501) | 2023 | Object | 3D Asset Collection, Annotation, Multimodal Learning   | 800K  | [Github](https://github.com/allenai/objaverse-xl)            | 800K+ free 3D object models with rich metadata (captions, tags, categories) and some objects include animations. |
| [DIVA-360](https://arxiv.org/abs/2307.16897) | 2023 | Object | 	Novel View Synthesis, NeRF Pretraining  | 50 | [Github](https://github.com/brown-ivl/DiVa360) | High-resolution synchronized multi-view video of dynamic table-scale scenes (53 RGB cameras), including hand-object interactions, segmentation masks, audio, and text descriptions. |
| [StrobeNet](https://arxiv.org/abs/2105.08016) | 2021 | Object | 3D Reconstruction        |  120K    | [Link](https://dzhange.github.io/StrobeNet/)  | Articulated-object categories providing many rendered RGB views plus joint + part segmentation and ground truth implicit / point cloud geometry to support animatable 3D reconstructions from sparse unposed images.  |
| [Amazon Berkeley Objects](https://arxiv.org/abs/2110.06199)  | 2021 | Object | 3D Reconstruction, Multi-view Retrieval, Material Estimation |   8K   | [Website](https://amazon-berkeley-objects.s3.amazonaws.com/index.html) | A large dataset of real household objects with high-resolution CAD models, PBR materials, real product images & metadata, enabling single-view 3D reconstruction, material estimation, & multi-view retrieval. |
| [Fusion 360 Gallery Dataset](https://www.research.autodesk.com/app/uploads/2023/03/Fusion_360_Gallery__A_Dataset_and_Environment_for_Programmatic_CAD_Construction_from_Human_Design_Sequences.pdf_recB1A7wJLthITzJo.pdf) | 2021 | Object | 3D reconstruction, segmentation, assembly prediction, sequential modeling |  8K    | [Github](https://github.com/AutodeskAILab/Fusion360GalleryDataset) | A parametric CAD dataset from real user submissions (≈20,000 designs) offering “sketch & extrude” construction sequences, operation-based face segmentation, and multi-part assemblies with joint and connectivity info. |
| [CO3Dv2](https://arxiv.org/abs/2109.00512)                   | 2021 | Object      | Novel View Synthesis, Category-level 3D Reconstruction       |  19K   | [Github](https://github.com/facebookresearch/co3d)           | A large-scale real-object dataset with object-centric multi-view images, annotated camera poses, and ground-truth 3D point clouds across 50 object categories. |
| [3D-FUTURE](https://arxiv.org/pdf/2009.09633.pdf)            | 2020 | Object      | Navigation, Exploration, Interaction                         |   10K   | [Github](https://github.com/3D-FRONT-FUTURE/3D-FUTURE-ToolBox) | A furniture CAD + texture dataset with nearly 10,000 detailed instances used in realistic room scenes, offering aligned textures for object pose, segmentation, and shape retrieval tasks. |
| [SketchGraphs](https://arxiv.org/abs/2007.08506) | 2020 | Object | - | 15M  | [Github](https://github.com/PrincetonLIPS/SketchGraphs) | A large-scale dataset of ~15M 2D parametric CAD sketches represented as geometric-constraint graphs to support generative modeling of sketches and prediction of likely constraints. |
| [ABC](https://openaccess.thecvf.com/content_CVPR_2019/papers/Koch_ABC_A_Big_CAD_Model_Dataset_for_Geometric_Deep_Learning_CVPR_2019_paper.pdf) | 2019 | Object      | Shape Analysis, Segmentation, Surface Fitting                |  1M    | [Link](https://deep-geometry.github.io/abc-dataset)          | A huge collection of CAD models with analytic parametric curves & surfaces, sharp feature annotations, patch decompositions, and ground truth differential geometry. |
| [ScanObjectNN](https://arxiv.org/abs/1908.04616) | 2019 | Object |   | 700 | [Link](https://hkust-vgd.github.io/scanobjectnn/) | Real-world indoor object point clouds (with background clutter, occlusion, partial scans) from SceneNN & ScanNet, over 15 categories. |
| [Thingi10K](https://arxiv.org/abs/1605.04797)                | 2016 | Object      | Scene Understanding, Semantic Segmentation, Layout Prediction |  300    | [Github](https://github.com/Thingi10K/Thingi10K)             | A collection of 10,000 real-world 3D printing meshes from Thingiverse, across 72 categories, with geometric issues like non-manifoldness and self-intersections included. |
| [A Large Dataset of Object Scans](https://vladlen.info/papers/3d-scan-dataset.pdf) | 2016 | Object      | Object Scanning, 3D Reconstruction, Object Categorization    |  10K    | [Github](https://github.com/isl-org/redwood-3dscan)          | A public domain dataset of 10,000+ consumer-grade real-object 3D scans, diverse in category and size. |
| [ShapeNet](https://arxiv.org/abs/1512.03012)             | 2015 | Object      | Single-view Reconstruction, Multi-view Reconstruction        |  300M    | [Link](https://shapenet.org/)                                | 3D CAD models (≈3M shapes), including ~220K models with classifications, part annotations, symmetry planes, alignments, physical size info. |
<!--
| [ModelNet](https://arxiv.org/pdf/1406.5670.pdf)              | CAD Models                                                   | 2015 | Object      | Classification, Segmentation, Retrieval, Reconstruction      |      | [Link](http://modelnet.cs.princeton.edu/#)                   |
| [PASCAL3D+](https://arxiv.org/pdf/1511.05175)                | CAD                                                          | 2014 | Object      | Scene Understanding, Object Detection, Semantic Segmentation |      | [Link](https://cvgl.stanford.edu/resources.html)             |
-->

### 🏙️ Scene

| Dataset                                                      | Year | Granularity | Tasks                                                        | Size | Site                                                         | Description                 
| ------------------------------------------------------------ | ---- | ----------- | ------------------------------------------------------------ | ---- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [InteriorGS](https://huggingface.co/datasets/spatialverse/InteriorGS) | 2025 | Scene<br> Indoor        | 3D scene understanding, controllable scene generation, embodied agent navigation |   100K   | [Hugging<br>Face](https://huggingface.co/datasets/spatialverse/InteriorGS) | A synthetic dataset with 100K procedurally generated indoor scenes, realistic object placement, simulated Aria-glass camera, full 6DoF trajectories, 3D floor-plans, 2D instance segmentation, and depth (range maps).
| [Aria Synthetic Environments](https://arxiv.org/abs/2306.06362)    | 2023 | Scene<br>Indoor         |  3D Question Answering, Spatial Reasoning, Scene Understanding  |   100K   |    [Link](https://facebookresearch.github.io/projectaria_tools/docs/open_datasets/aria_digital_twin_dataset?utm_source=chatgpt.com)   | A synthetic dataset with 100K procedurally generated indoor scenes, realistic object placement, simulated Aria-glass camera, full 6DoF trajectories, 3D floor-plans, 2D instance segmentation, and depth (range maps). |
| [DL3DV-10K](https://arxiv.org/abs/2312.16256) | 2023 | Scene | Novel View Synthesis, NeRF Pretraining | 10K | [Website](https://dl3dv-10k.github.io/DL3DV-10K/) | A large real-world multi-view video dataset capturing 10,510 4K videos across 65 kinds of POI scenes, annotated for complexity (reflection, transparency, lighting, texture) to support generalizable novel view synthesis and NeRF research.
| [Aria Digital Twin](https://arxiv.org/abs/2306.06362)        | 2023 | Scene<br>Indoor         | 3D Question Answering, Spatial Reasoning, Scene Understanding |   400   | [Link](https://facebookresearch.github.io/projectaria_tools/docs/open_datasets/aria_digital_twin_dataset?utm_source=chatgpt.com) | An egocentric dataset captured with wearable glasses, offering synchronized RGB + monocrome cameras, IMU, full sensor calibration, depth maps, 6-DoF poses (device & object), human pose & eye gaze, segmentation & synthetic renderings. |
| [PointOdyssey](https://arxiv.org/abs/2307.15055)             | 2023 | Scene | 3D Generation, Multimodal Learning, Simulation |  104  | [Link](https://pointodyssey.com/)                     | A synthetic dataset with natural motion, deformable characters, diverse scenes & materials, and long videos for fine-grained point-tracking evaluation. |
| [ScanNet++](https://arxiv.org/abs/2308.11417) | 2023 | Scene<br>Indoor |  | 1K | [Website](https://kaldir.vc.in.tum.de/scannetpp/) | A high-fidelity indoor scene dataset with sub-mm laser scans, high-res DSLR + iPhone RGB-D captures, dense mesh & semantic + instance annotations, supporting novel view synthesis & scene understanding. 
| [Kubric](https://arxiv.org/abs/2203.03570)                   | 2022 | Mixed  | Semantic Mapping, 2.5D Reconstruction, View-consistent Semantics |   N/A   | [Github](https://github.com/google-research/kubric)          | Kubric is a framework for generating photo-realistic synthetic scenes in Python (via Blender + PyBullet), with rich annotations (depth, segmentation, bounding boxes, camera pose, optical flow, etc.), scalable to TBs of data. |
| [HM3D](https://arxiv.org/abs/2109.08238) | 2021 | Scene<br>Indoor |  | 1K |  |High-fidelity set of 1,000 real-world indoor 3D meshes with extensive navigable space, clean reconstructions, and textured geometry. |
| [HyperSim](https://arxiv.org/abs/2011.02523)                 |  2021 | Scene<br>Indoor  | Multi-task Scene Understanding                               |   461   | [Github](https://github.com/apple/ml-hypersim)     | A photorealistic synthetic indoor dataset with full scene geometry + materials + lighting, dense per-pixel semantic + instance segmentation, and detailed lighting decomposition. |
| [Habitat 2.0](https://arxiv.org/pdf/2106.14405)              | 2021 | Scene<br>Indoor      | Pick, Place, Navigate, Open, Close, Rearrange                | 111 | [Link](https://sites.google.com/view/habitat2)               | A reconfigurable, artist-authored indoor dataset of apartments with articulated objects, semantic class and surface annotations, collision proxies, matching real layout footprints. |
| [Virtual KITTI2](https://arxiv.org/abs/2001.10773)            | 2020 | Scene<br>Outdoor         | 6D Pose Estimation, Object Detection, Benchmarking           |   5    | [Link](https://datasetninja.com/virtual-kitti)               | Virtual KITTI is a synthetic driving-scene dataset with fully annotated RGB, depth, optical flow, semantic & instance segmentation, and variants in weather/camera conditions using cloned sequences from KITTI. | 
| [RELLIS-3D](https://arxiv.org/abs/2011.12954)                | 2020 | Scene<br>Outdoor | 3D Semantic Segmentation, Sensor Fusion, Autonomous Navigation |   13K   | [Website](https://www.unmannedlab.org/research/RELLIS-3D)    | A multimodal off-road robotics dataset with 13,556 LiDAR scans, 6,235 RGB images, point-wise & pixel-wise semantic labels over 20 classes, plus stereo, GPS/IMU, and camera-LiDAR calibrated data. |
| [3D-FRONT](https://openaccess.thecvf.com/content/ICCV2021/papers/Fu_3D-FRONT_3D_Furnished_Rooms_With_layOuts_and_semaNTics_ICCV_2021_paper.pdf?utm_source=chatgpt.com) | 2020 | Scene<br>Indoor         | Scene Understanding, Layout Analysis, Object Arrangement     |   18K   | [HuggingFace](https://huggingface.co/datasets/huanngzh/3D-Front) | Synthetic indoor scene dataset with professionally designed layouts, high-quality textured furniture models, consistent style curation, and semantic annotations. |
| [Structured3D](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123540494.pdf) | 2020 | Scene<br>Indoor         | Reconstruction, Segmentation, Object Detection               |   3.5K   | [Link](https://structured3d-dataset.org/#download)           | Structured3D provides synthetic photo-realistic indoor scenes with rich “primitive + relationship” structure annotations (planes, lines, junctions, room layouts, floorplans), plus depth maps, semantic masks, and varied lighting / furnishing configurations. |
| [Mapillary](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123470579.pdf) | 2020 | Scene<br>Outdoor         | Reconstruction, Semantics, Viewpoint Estimation              |  1.6M    | [Link](https://www.mapillary.com/dataset/depth)              | A large street-level image sequence dataset with 1.6M geo-tagged images, covering diverse cities, seasons, weather, and appearance changes for lifelong place recognition. |
| [BlendedMVS](https://arxiv.org/abs/1911.10127)               | 2019 | Scene      | Reconstruction, Alignment, Evaluation                        |  113    | [Github](https://github.com/YoYo000/BlendedMVS)              | Multi-view stereo, offering 113 textured mesh scenes, rendered + blended image inputs, and ground-truth depth maps to improve generalization. |
| [Replica](https://arxiv.org/abs/1906.05797)                  | 2019 | Scene<br>Indoor  | Scene Graph Generation, Object Detection, Relationship Modeling |  18    | [Github](https://github.com/facebookresearch/Replica-Dataset) | 18 photo-realistic indoor scenes with dense meshes, HDR textures, semantic & instance annotations, plus mirror and glass reflectors.  |
| [RealEstate10K](https://arxiv.org/abs/1805.09817)            | 2018 | Scene         | Part Segmentation, Hierarchical Labeling, Shape Understanding |  10K    | [Link](https://google.github.io/realestate10k/)              | Camera trajectories from ~10,000 YouTube real-estate videos, with pose + intrinsics data for 10 million frames over ~80,000 clips. |
| [MegaDepth](https://www.cs.cornell.edu/projects/megadepth/paper.pdf) | 2018 | Scene         | Multisensory Perception, Object Interaction, Representation Learning |   200   | [Link](https://www.cs.cornell.edu/projects/megadepth/)       | Diverse scene-depth dataset built from Internet multi-view photo collections, offering ~130K images with dense depth / ordinal depth labels from ~200 reconstructed scenes. |
| [DeepMVS](https://arxiv.org/pdf/1804.00650)                  | 2018 | Scene         | CAD Alignment, 3D Matching, Pose Estimation                  |   120   | [Link](https://phuang17.github.io/DeepMVS/mvs-synth.html)    | A photorealistic synthetic multi-view dataset (MVS-SYNTH: 120 urban sequences, 100 frames each, with ground truth disparities + full camera calibration) plus real indoor/outdoor image sets, for training disparity prediction in MVS. |
| [ScanNet](https://arxiv.org/abs/1702.04405)                  | 2017 | Scene<br>Indoor  | Feature Matching, Registration, 3D Reconstruction            |   1.5K   | [Link](http://www.scan-net.org/)                             | An indoor RGB-D scene dataset with 1,513 scans across 707 spaces, ~2.5 million frames, dense surface reconstructions, semantic + instance labels, and aligned CAD models. |
| [Matterport3D](https://arxiv.org/abs/1709.06158) | 2017 | Scene<br>Indoor |  |  90  | [Website](https://matterport.com/)  | Indoor RGB-D dataset with 90 scenes, 194,400 RGB-D images, textured meshes and semantic/instance annotations. |
| [Semantic3D](https://isprs-annals.copernicus.org/articles/IV-1-W1/91/2017/isprs-annals-IV-1-W1-91-2017.pdf) | 2016 | Scene<br>Outdoor         | Point Cloud Classification, Semantic Segmentation            |   30   | [Link](http://www.semantic3d.net/)         | An outdoor laser-scanned benchmark of ~30 high-density static scans (≈4 B points), with manual semantic labels across 8 classes. | 
| [SceneNN / ObjectNN](https://www.saikit.org/static/projects/sceneNN/home/pdf/dataset_3dv16.pdf) | 2016 | Scene<br>Indoor  | Multi-view Fusion, 3D Reconstruction, Semantic Segmentation  |  100    | [Link](https://hkust-vgd.github.io/scenenn/)                 | An indoor RGB-D scene dataset with ≈100 reconstructed scenes into triangle meshes; per-vertex, per-pixel semantic and instance annotations; also provides bounding boxes (axis-aligned & oriented) and object poses. |
| [Virtual KITTI2](https://arxiv.org/abs/1605.06457)            | 2016 | Scene<br>Outdoor         |          |   35    | [Link](http://www.xrce.xerox.com/Research-Development/Computer-Vision/Proxy-Virtual-Worlds)               | A photo-realistic synthetic video dataset cloned from KITTI, with automatic ground truth for object detection/tracking, scene & instance segmentation, depth, optical flow, and with weather & camera-angle variants. | 

 

### 📊 Modalities of 3D datasets 

> ✅ indicates supported modality, * indicates CAD mesh
> 
> 📝 *Modality includes available signals like RGB, Depth, Pose, Segmentation, Flow, Mesh, Action...*


| Dataset                        | RGB-D | Point Cloud | Mesh | Multi-view | Voxel | Implicit Field |
|--------------------------------|-------|-------------|------|------------|----------|----------------|
| GigaHands                      | ❌    | ❌          | ✅   | ✅         |❌             |❌              |
| InteriorGS                     |  ✅   | ❌          | ❌   | ✅         |❌             |❌              |
| HPSketch                       | ❌    | ❌          | ❌   | ❌         |❌             | ❌             |
| CBF                            | ❌    | ❌          | ❌   | ❌         |❌             | ❌             |
| Parametric 20000               | ❌    | ✅          | ✅<sup>*</sup>   | ❌         |❌             | ❌             |
| WildRGB-D                      | ✅    | ✅          | ❌   |  ✅        |❌             | ❌             |
| BRep2seq                       | ❌    | ❌          | ✅<sup>*</sup>   | ❌         |❌             | ❌             |
| Aria Synthetic Environments    |  ✅   |  ❌         | ❌   | ❌         |❌             | ❌             |
| DL3DV-10K                      | ❌    | ❌          | ❌   |  ✅         |❌             |  ❌           |
| PointOdyssey                   | ❌    |    ❌      |  ✅   |    ✅      |❌             | ❌             |
| Aria Digital Twin              | ✅    | ❌          | ❌   | ✅         |❌             | ❌             |
| ScanNet++                      | ✅    | ✅          | ✅   | ✅         |❌             | ❌             |
| Objaverse                      | ❌    | ❌          | ✅   | ❌         |❌             |  ❌            |
| DIVA-360                       | ❌    | ❌          |❌   | ✅          |❌             | ❌             |
| H3WB                           | ❌    | ❌          | ❌   |  ✅        |❌              | ❌             |
| Kubric                         | ✅     | ✅          | ✅    | ✅         |❌             | ❌             |
| Amazon Berkeley Objects        | ❌    | ❌          | ✅<sup>*</sup>   | ✅        |❌              | ❌             |
| HM3D                           | ❌    | ❌          | ✅   | ❌         |❌             | ❌             |
| Fusion 360 Gallery Dataset     | ❌    | ❌          | ✅<sup>*</sup>   | ❌         |❌             | ❌             |
| CO3Dv2                         | ❌    | ✅          | ❌   | ✅         |❌             | ❌             |
| HyperSim                       | ✅    | ❌          | ❌    | ✅        |❌             | ❌             |
| Habitat 2.0                    |  ❌    | ❌          | ✅   | ❌         |❌             | ❌             |
| StrobeNet                      | ❌    | ✅          | ❌   | ✅         |❌             | ✅             |
| Virtual KITTI 2                | ✅    | ❌          | ❌   |   ❌        |❌             | ❌             |
| RELLIS-3D                      | ❌    | ✅          | ❌   | ❌         |❌             | ❌             |
| FaceScape                      | ❌    | ❌          | ✅   | ✅       |❌              | ❌             |
| A Large Dataset of Object Scans| ✅    | ✅          | ❌   | ❌         |❌             | ❌             |
| 3D-FRONT                       | ❌    | ❌          | ✅<sup>*</sup>   | ❌         |❌             | ❌             |
| 3D-FUTURE                      | ❌    | ❌          | ✅<sup>*</sup>   | ❌         |❌             | ❌             |
| SketchGraphs                   | ❌    | ❌          | ❌   | ❌         |❌             | ❌             |
| Structured3D                   | ✅    | ❌          | ✅   | ✅        |❌              | ❌             |
| Mapillary                      | ❌    | ❌          | ❌   | ✅        |❌              | ❌             |
| ScanObjectNN                   | ❌    | ✅          | ❌   |   ❌       |❌             | ❌             |
| ABC                            | ❌    | ❌          | ✅<sup>*</sup>   | ❌        | ✅         | ❌             |
| BlendedMVS                     |  ✅    | ❌          | ✅   | ✅        |❌             | ❌             |
| Replica                        | ❌    | ❌          | ✅   | ❌        |❌              | ❌             |
| RealEstate10K                  | ❌    | ❌          | ❌   | ✅         |❌             | ❌             |
| MegaDepth                      | ✅    | ❌          | ❌   | ✅         |❌             | ❌             |
| DeepMVS                        | ✅    | ❌          | ❌   |  ❌        |❌             | ❌             |
| ScanNet                        | ✅    | ✅          | ✅   | ✅         |❌             | ❌             |
| Matterport3D                   | ✅    | ❌          | ✅   | ❌       |❌               | ❌             |
| Thingi10K                      | ❌    | ❌          | ✅<sup>*</sup>   | ❌         | ✅        | ❌             |
| Semantic3D                     | ❌    | ✅          | ❌   | ❌        |❌              | ❌             |
| SceneNN / ObjectNN             | ✅    | ✅          | ✅   | ✅        |❌              | ❌             |
| A Large Dataset of Object Scans| ❌    | ✅          | ✅   | ❌        |❌              | ❌             |
| Virtual KITTI                  | ✅    | ❌          | ❌   | ❌        |❌              | ❌             |
| ShapeNet                       | ❌    | ❌          | ✅<sup>*</sup>   | ❌         | ✅        | ❌             |

## ⚒️ Applications

### 🔄 3D Reconstruct

| Title | Year | Paper | Website | Code | HuggingFace
| :--- | :--- | :--- | :--- | :--- | :--
| DUSt3R: Geometric 3D Vision Made Easy | 2024 | [📄 Paper](https://arxiv.org/abs/2312.14132) | [🌍 Website](https://europe.naverlabs.com/research/publications/dust3r-geometric-3d-vision-made-easy/) | [💾 Code](https://github.com/naver/dust3r) | -
| VGGT: Visual Geometry Grounded Transformer | 2025 | [📄 Paper](https://arxiv.org/abs/2503.11651) | [🌍 Website](https://vgg-t.github.io/) | [💾 Code](https://github.com/facebookresearch/vggt) | [😊 HuggingFace](https://huggingface.co/spaces/facebook/vggt) |
| $\pi^3$: Scalable Permutation-Equivariant Visual Geometry Learning | 2025 | [📄 Paper](https://arxiv.org/abs/2507.13347) | [🌍 Website](https://yyfz.github.io/pi3/) | [💾 Code](https://github.com/yyfz/Pi3) | [😊 HuggingFace](https://huggingface.co/spaces/yyfz233/Pi3) |
| MV-DUSt3R+: Single-Stage Scene Reconstruction from Sparse Views In 2 Seconds | 2024 | [📄 Paper](https://arxiv.org/abs/2412.06974) | [🌍 Website](https://mv-dust3rp.github.io/) | [💾 Code](https://github.com/facebookresearch/mvdust3r) | - |
| MoGe-2: Accurate Monocular Geometry with Metric Scale and Sharp Details | 2025 | [📄 Paper](https://arxiv.org/abs/2507.02546) | - | - | - |
| MASt3R: Grounding Image Matching in 3D | 2024 | [📄 Paper](https://arxiv.org/abs/2406.09756) | [🌍 Website](https://europe.naverlabs.com/blog/mast3r-matching-and-stereo-3d-reconstruction/) | [💾 Code](https://github.com/naver/mast3r) | [😊 HuggingFace](https://huggingface.co/spaces/naver/MASt3R)
| Mickey: Matching 2D Images in 3D: Metric Relative Pose from Metric Correspondences | 2024 | [📄 Paper](https://arxiv.org/abs/2404.06337) | [🌍 Website](https://nianticlabs.github.io/mickey/) | [💾 Code](https://github.com/nianticlabs/mickey) | -
| StreamVGGT: Streaming 4D Visual Geometry Transformer | 2025 | [📄 Paper](https://arxiv.org/abs/2507.11539) | [🌍 Website](https://wzzheng.net/StreamVGGT/) | [💾 Code](https://github.com/wzzheng/StreamVGGT) | [😊 HuggingFace](https://huggingface.co/spaces/lch01/StreamVGGT)
| MoVieS: Motion-Aware 4D Dynamic View Synthesis in One Second | 2025 | [📄 Paper](https://arxiv.org/abs/2507.10065) | [🌍 Website](https://chenguolin.github.io/projects/MoVieS/) | [💾 Code](https://github.com/chenguolin/MoVieS) | -

### ✨ 3D Generation

| Title | Year | Paper | Website | Code | HuggingFace
| :--- | :--- | :--- | :--- | :--- | :--
| DreamFusion: Text-to-3D using 2D Diffusion | 2022 | [📄 Paper](https://arxiv.org/abs/2209.14988) | [🌍 Website](https://dreamfusion3d.github.io/) | - | -
| Magic3D: High-Resolution Text-to-3D Content Creation | 2023 | [📄 Paper](https://arxiv.org/abs/2211.10440) | [🌍 Website](https://research.nvidia.com/labs/dir/magic3d/) | - | -
| DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation | 2024 | [📄 Paper](https://arxiv.org/abs/2309.16653) | [🌍 Website](https://dreamgaussian.github.io/) | [💾 Code](https://github.com/dreamgaussian/dreamgaussian) | [😊 HuggingFace](https://huggingface.co/spaces/jiawei011/dreamgaussian)
| DreamMesh: Jointly Manipulating and Texturing Triangle Meshes for Text-to-3D Generation | 2025 | [📄 Paper](https://arxiv.org/abs/2409.07454) | [🌍 Website](https://dreammesh.github.io/) | - | -
| Progressive Rendering Distillation: Adapting Stable Diffusion for Instant Text-to-Mesh Generation without 3D Data | 2025 | [📄 Paper](https://arxiv.org/abs/2503.21694) | [🌍 Website](https://theericma.github.io/TriplaneTurbo/) | [💾 Code](https://github.com/theEricMa/TriplaneTurbo) | [😊 HuggingFace](https://huggingface.co/spaces/ZhiyuanthePony/TriplaneTurbo)
| MVDream: Multi-view Diffusion for 3D Generation | 2024 | [📄 Paper](https://arxiv.org/abs/2308.16512) | [🌍 Website](https://mv-dream.github.io/) | [💾 Code](https://github.com/bytedance/MVDream) | - 
| Structured 3D Latents for Scalable and Versatile 3D Generation | 2025 | [📄 Paper](https://arxiv.org/abs/2412.01506) | [🌍 Website](https://microsoft.github.io/TRELLIS/) | [💾 Code](https://github.com/Microsoft/TRELLIS) | [😊 HuggingFace](https://huggingface.co/spaces/trellis-community/TRELLIS)
| 3D-SceneDreamer: Text-Driven 3D-Consistent Scene Generation | 2024 | [📄 Paper](https://arxiv.org/abs/2403.09439) | - | - | -

### 🎬 Video Generation

| Title | Year | Paper | Website | Code | HuggingFace
| :--- | :--- | :--- | :--- | :--- | :--
| CogVideoX: Text-to-Video Diffusion Models with An Expert Transformer | 2024 | [📄 Paper](https://arxiv.org/abs/2408.06072) | [🌍 Website](https://yzy-thu.github.io/CogVideoX-demo/) | [💾 Code](https://github.com/zai-org/CogVideo) | [😊 HuggingFace](https://huggingface.co/spaces/zai-org/CogVideoX-5B-Space)
| Wan: Open and Advanced Large-Scale Video Generative Models | 2025 | [📄 Paper](https://arxiv.org/abs/2503.20314) | [🌍 Website](https://wan.video/) | [💾 Code](https://github.com/Wan-Video/Wan2.1)| [😊 HuggingFace](https://huggingface.co/Wan-AI)
| Lumiere: A Space-Time Diffusion Model for Video Generation | 2024 | [📄 Paper](https://arxiv.org/abs/2401.12945) | [🌍 Website](https://lumiere-video.github.io/) | [💾 Code](https://github.com/lumiere-video/lumiere-video.github.io) | -
| Emu Video: Factorizing Text-to-Video Generation by Explicit Image Conditioning | 2024 | [📄 Paper](https://arxiv.org/abs/2311.10709) | [🌍 Website](https://emu-video.metademolab.com/) | - | -
| Stable Video Diffusion: Scaling Latent Video Diffusion Models to Large Datasets | 2023 | [📄 Paper](https://arxiv.org/abs/2311.15127) | [🌍 Website](https://sv4d20.github.io/) | [💾 Code](https://github.com/Stability-AI/generative-models) | [😊 HuggingFace](https://huggingface.co/stabilityai/sv4d2.0)
| 3D-Aware Video Generation | 2023 | [📄 Paper](https://arxiv.org/abs/2206.14797) | [🌍 Website](https://sherwinbahmani.github.io/3dvidgen/) | [💾 Code](https://github.com/sherwinbahmani/3dvideogeneration/) | -
| World-consistent Video Diffusion with Explicit 3D Modeling | 2024 | [📄 Paper](https://arxiv.org/abs/2412.01821) | [🌍 Website](https://zqh0253.github.io/wvd/) | - | -
| IM-Portrait: Learning 3D-aware Video Diffusion for Photorealistic Talking Heads from Monocular Videos | 2025 | [📄 Paper](https://arxiv.org/abs/2504.19165) | [🌍 Website](https://y-u-a-n-l-i.github.io/projects/IM-Portrait/) | - | -
| Geometry Forcing: Marrying Video Diffusion and 3D Representation for Consistent World Modeling | 2025 | [📄 Paper](https://arxiv.org/abs/2507.07982) | [🌍 Website](https://geometryforcing.github.io/) | - | - 
| Force Prompting: Video Generation Models Can Learn and Generalize Physics-based Control Signals | 2025 | [📄 Paper](https://arxiv.org/abs/2505.19386) | [🌍 Website](https://force-prompting.github.io/) | [💾 Code](https://github.com/brown-palm/force-prompting) | -
| PhysGen: Rigid-Body Physics-Grounded Image-to-Video Generation | 2024 | [📄 Paper](https://arxiv.org/abs/2409.18964) | [🌍 Website](https://stevenlsw.github.io/physgen/) | [💾 Code](https://github.com/stevenlsw/physgen) | -
| Tora: Trajectory-oriented Diffusion Transformer for Video Generation | 2025 | [📄 Paper](https://arxiv.org/abs/2407.21705) | [🌍 Website](https://ali-videoai.github.io/tora_video/) | [💾 Code](https://github.com/alibaba/Tora) | [😊 HuggingFace](https://huggingface.co/Alibaba-Research-Intelligence-Computing/Tora)
| CamI2V: Camera-Controlled Image-to-Video Diffusion Model | 2024 | [📄 Paper](https://arxiv.org/abs/2410.15957) | [🌍 Website](https://zgctroy.github.io/CamI2V/) | [💾 Code](https://github.com/ZGCTroy/CamI2V) | [😊 HuggingFace](https://huggingface.co/MuteApo/CamI2V/tree/main)

### 🌐 World Models

| Title | Year | Paper | Website | Code | HuggingFace
| :--- | :--- | :--- | :--- | :--- | :--
| Learning to Simulate Complex Physics with Graph Networks | 2020 | [📄 Paper](https://arxiv.org/abs/2002.09405) | [🌍 Website](https://sites.google.com/view/learning-to-simulate/) | [💾 Code](https://github.com/google-deepmind/deepmind-research/tree/master/learning_to_simulate) | - 
| Learning Particle Dynamics for Manipulating Rigid Bodies, Deformable Objects, and Fluids | 2019 | [📄 Paper](https://arxiv.org/abs/1810.01566) | [🌍 Website](http://dpi.csail.mit.edu/) | [💾 Code](https://github.com/YunzhuLi/DPI-Net) | -
| Learning Mesh-Based Simulation with Graph Networks | 2021 | [📄 Paper](https://arxiv.org/abs/2010.03409) | [🌍 Website](https://sites.google.com/view/meshgraphnets) | [💾 Code](https://github.com/google-deepmind/deepmind-research/tree/master/meshgraphnets) | - 
| SoftGym: Benchmarking Deep Reinforcement Learning for Deformable Object Manipulation | 2021 | [📄 Paper](https://arxiv.org/abs/2011.07215) | [🌍 Website](https://sites.google.com/view/softgym) | [💾 Code](https://github.com/Xingyu-Lin/softgym) | - 
| 3D Gaussian Splatting for Real-Time Radiance Field Rendering | 2023 | [📄 Paper](https://arxiv.org/abs/2308.04079) | [🌍 Website](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/) | [💾 Code](https://github.com/graphdeco-inria/gaussian-splatting) | - 
| Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis | 2023 | [📄 Paper](https://arxiv.org/abs/2308.09713) | [🌍 Website](https://dynamic3dgaussians.github.io/) | [💾 Code](https://github.com/JonathonLuiten/Dynamic3DGaussians) | - 
| 4D Gaussian Splatting for Real-Time Dynamic Scene Rendering | 2024 | [📄 Paper](https://arxiv.org/abs/2310.08528) | [🌍 Website](https://guanjunwu.github.io/4dgs/) | [💾 Code](https://github.com/hustvl/4DGaussians) | - 
| Gaussian Splatting SLAM | 2024 | [📄 Paper](https://arxiv.org/abs/2312.06741) | [🌍 Website](https://rmurai.co.uk/projects/GaussianSplattingSLAM/) | [💾 Code](https://github.com/muskie82/MonoGS) | -
| Splat-SLAM: Globally Optimized RGB-only SLAM with 3D Gaussians | 2024 | [📄 Paper](https://arxiv.org/abs/2405.16544) | - | [💾 Code](https://github.com/google-research/Splat-SLAM) | -
| ParticleFormer: A 3D Point Cloud World Model for Multi-Object, Multi-Material Robotic Manipulation | 2025 | [📄 Paper](https://arxiv.org/abs/2506.23126) | [🌍 Website](https://suninghuang19.github.io/particleformer_page/) | - | -

## 👥 Contributors

We welcome contributions! If you'd like to contribute, please submit a pull request or open an issue.  

- [Hongyang Du](https://hongyang-du.github.io)  