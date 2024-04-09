---
title: 'Access detection measurements from a QuPath in python'
date: 2024-04-09
permalink: /posts/2024/04/09/
tags:
  - QuPath
  - paquo
---

Access detection measurements from a QuPath project in python.  
------
Iterate over each image, and, each annotation per image, to access the detections and their measurements. Put the measurements in a pandas *dataframe*.

### Example

```python

"""
example showing how to get detections for each annotation of an image within a project

Created on Tue Apr  9 13:53:22 2024

@author: zalavadia.ajay@gmail.com
"""
from paquo.projects import QuPathProject
import pandas as pd

EXAMPLE_PROJECT = "D:\\_TestFiles\\test-project\\project.qpproj"

with QuPathProject(EXAMPLE_PROJECT, mode='r') as qp:
    print("Project Name: ", qp.name)
    # iterate over the images
    for image in qp.images:
        # annotations and detections are accessible via the hierarchy
        annotations = image.hierarchy.annotations
        detections = image.hierarchy.detections

        if(len(detections)>0):
            for annotation in annotations: 
                # list Comprehension
                childrens = [detection for detection in detections if detection.parent.name == annotation.name]
                # measurements dictionary for each detection
                df = pd.DataFrame(detection.measurements for detection in childrens)
                # print the total number of detections and the total number of measurements
                print(annotation.name ,"--> Number of detections: ", df.shape[0], " Number of measurements: ", df.shape[1])
```

### Links with more infomration about paquo:

- <https://paquo.readthedocs.io/en/latest/index.html>
- <https://github.com/Bayer-Group/paquo>

### Installation and setup notes:

  1. Create conda environment
  2. Install ***paquo***
  3. Update config file with path to ***QuPath*** installation directory
  4. Install ***spyder*** IDE

> I had some trouble using ***paquo*** via PyCharm IDE, more investigations needed for troubleshooting
