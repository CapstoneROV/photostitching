# Photo Stitching Module
**Author :** [Pi Ko](https://paingthet.com/) ([pk2269@nyu.edu](mailto:pk2269@nyu.edu))

![Image of Version](https://img.shields.io/badge/version-v1.0-green)
![Image of Dependencies](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen)
[![forthebadge](https://forthebadge.com/images/badges/works-on-my-machine.svg)](https://forthebadge.com)

[![forthebadge](https://forthebadge.com/images/badges/made-with-python.svg)](https://forthebadge.com)

A Python package for RoV Image Stitching.

Based on opencv's [stitching
module](https://github.com/opencv/opencv/tree/4.x/modules/stitching)

## Installation

use the [docker image](#docker-cli)

or `pip` to install `stitching` from
[PyPI](https://pypi.org/project/stitching/).

```bash
pip install stitching
```

## Usage

```python
stitch.py [Directory]\*.png -v --confidence_threshold=0.9 --detector="orb"
```

Important Notes:
- The images must have a signifiant overlap
- Must adjust the confidence threshold or use a new detector if it fails

# I/O Results

![Demo](inputoutput.png)


# Processing and Output

### Feature Extraction
![Demo](results/01_features_img1.jpg)
![Demo](results/01_features_img2.jpg)

### Matching Features
![Demo](results/02_matches_img2_to_img4.jpg)

### Seam Masking
![Demo](results/08_seam_mask1.jpg)
![Demo](results/08_seam_mask3.jpg)


### Results
![Demo](results/09_result_with_seam_lines.jpg)
![Demo](results/09_result_with_seam_polygons.jpg)
