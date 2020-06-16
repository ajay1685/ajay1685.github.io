---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* B.S. in Pharmacy, Rajiv Gandhi University of Health Sciences, 2007
* M.S. in Analytical Chemistry, Governors State University, 2009
* Ph.D in Clinical Bio-Analytical Chemistry, Cleveland State University, 2018

Work experience
======
* 2018-present: Imaging Specialist
  * Imaging Core, Lerner Reserach Institute
  * Duties included: Provide imaging consulation and training for confocal, TIRF, multispectral and scanning electron microscopy. Offer image processing and data analysis support to biomedical researchers. Develop and maintain billing software for the imaging core to manage access, track usage and logg accounting information.  

* 2012-2015: Research Assistant
  * Cleveland State University
  * Duties included: Supervise operations and maintain Scanning Electron Microscope (SEM) Facility. Provide support and teach labs for SEM and EDS analysis to graduate and undergraduate students.
  
Skills
======
* Microscopy (Confocal, TIRF, multi-photon and multispectral)
* Image processing (ImageJ, QuPath, Volocity, Digital Micrograph, Image-Pro, HALO)
  * Whole slide multispectral image analysis
  * 3D volume processing for confocal z-stacks
  * Tracking cells for timelapse imaging 
* Machine learning and data anaysis
  * Train models for segemntation of cells and idetify regions for the whole slide images

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Lead developer for the core billing software and iLab integration.
