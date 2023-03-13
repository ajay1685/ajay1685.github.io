---
title: 'Resonance scanners are cool again, thanks to the Noise2Void'
date: 2023-02-01
permalink: /posts/2023/02/01/
tags:
  - Resonance scanner
  - live imaging
  - Denoising
---

Video-rate confocal imaging using resonance scanners followed by post processing using the Noise2Void.
------
  Resonance scanners have been around for some time but have not been very popular. Resonance scanners are designed to enable high speed acquisition for scanning systems. Images acquired with resonance scanner often requires frame averaging or frame integrations due to the amount of noise present in a single scan. The frame averaging or the frame integration will reduce the speed at which images can be captured. This hindered the wide spread use and adoption of the resonance scanners for live imaging. We can use Noise2Void to clean up the noisy images acquired at full speed of the resonance scanner. On a Leica SP8 Laser Scanning Confocal Microscope equipped with resonace scanners, we can acquire time-lapse movies at video-rate (27 fps).

Here is an example of such acquition:

  Time-lapse acquisition of red blood cells flowing at high speed through vasculature in a zebra fish. This time-lapse data were acquired on a Leica SP8 Laser Scanning Confocal Microscope equipped with resonance scanners, using a 25x water immersion lens.
<video src="https://user-images.githubusercontent.com/10900214/216131637-ffdb309c-7df5-4824-9eff-f3f5eb549f7f.mp4" controls="controls" style="max-width: 650px;">
</video>

Link to Noise2Void Paper: https://arxiv.org/abs/1811.10980
  
---
Author: Ajay Zalavadia


