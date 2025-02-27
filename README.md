## CrowdPose: Efficient Crowded Scenes Pose Estimation and A New Benchmark

## Citation
    @article{li2018crowdpose,
      title={CrowdPose: Efficient Crowded Scenes Pose Estimation and A New Benchmark},
      author={Li, Jiefeng and Wang, Can and Zhu, Hao and Mao, Yihuan and Fang, Hao-Shu and Lu, Cewu},
      journal={arXiv preprint arXiv:1812.00324},
      year={2018}
    }


## Introduction
This is a fork repository of [CrowdPose](https://github.com/Jeff-sjtu/CrowdPose) with Python 3.9 compatibility.
It does not guarantee backward compatibility.
You can build by below command at crowdpose-api/PythonAPI directory:
``` shell
python3 setup.py install # option 1
pip install . # option 2
```

Below text is the same as the original repo.

## Code
We provide [evaluation tools](crowdpose-api) for CrowdPose dataset. Our evaluation tools is developed based on [@cocodataset/cocoapi](https://github.com/cocodataset/cocoapi). The source code of our model has been integrated into [AlphaPose](https://github.com/MVIG-SJTU/AlphaPose/tree/pytorch).

## Dataset
[Train + Validation + Test Images](https://drive.google.com/file/d/1VprytECcLtU4tKP32SYi_7oDRbw7yUTL/view?usp=sharing) (Google Drive)

[Annotations](https://drive.google.com/drive/folders/1Ch1Cobe-6byB7sLhy8XRzOGCGTW2ssFv?usp=sharing) (Google Drive)

## Results

**Results on CrowdPose Validation:**

*Compare with state-of-the-art methods*
<center>

| Method | AP @0.5:0.95 | AP @0.5 | AP @0.75 | AR @0.5:0.95 | AR @0.5 | AR @0.75 |
|:-------|:-----:|:-------:|:-------:|:-------:|:-------:|:-------:|
| Detectron (Mask R-CNN) | 57.2 | 83.5 | 60.3 | 65.9 | 89.3 | 69.4 |
| Simple Pose (Xiao *et al.*) | 60.8 | 81.4 | 65.7 | 67.3 | 86.3 | 71.8 |
| **Ours** | **66.0** | **84.2** | **71.5** | **72.7** | **89.5** | **77.5** |

</center>

*Compare with open-source systems*
<center>

| Method | AP @*Easy* | AP @*Medium* | AP @*Hard* | FPS |
|:-------|:-----:|:-------:|:-------:|:-------:|
| OpenPose (CMU-Pose) | 62.7 | 48.7 | 32.3 | 5.3 |
| Detectron (Mask R-CNN) | 69.4 | 57.9 | 45.8 | 2.9 |
| **Ours** | **75.5** | **66.3** | **57.4** | **10.1** |

</center>

**Results on MSCOCO Validation:**
<center>

| Method | AP @0.5:0.95 | AR @0.5:0.95 |
|:-------|:-----:|:-------:|
| Detectron (Mask R-CNN) | 64.8 | 71.1 |
| Simple Pose (Xiao *et al.*) | 69.8 | 74.1 |
| **AlphaPose** | **70.9** | **76.4** |

</center>

## Contributors
 CrowdPose is authored by [Jiefeng Li](http://jeff-leaf.site/), [Can Wang](https://github.com/Canwang-sjtu), [Hao Zhu](https://github.com/BernieZhu), [Yihuan Mao](), [Hao-Shu Fang](https://fang-haoshu.github.io/), and [Cewu Lu](http://www.mvig.org/).
