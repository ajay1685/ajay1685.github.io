---
title: 'Access detection measurements from a QuPath project in python'
date: 2026-08-13
permalink: /posts/2026/08/13/
tags:
  - Histology
  - Collagen
  - Picrosirius red
---

When the red is too dark for Picrosirius red staining in histology.  
------

The information regarding the Picrosirius red (PSR) staining protocols, the dye identity, and the concentration variations is based on foundational histological literature and biological stain certification standards.

Here are the primary sources:

### 1. Protocol history and Dye Identity

1. **Sweat and Puchtler et al. (1964):** 


2. **Puchtler et al. (1973):** The original standard picro-sirius red method for staining collagen was developed by Sweat, Puchtler, and colleagues. This protocol established the use of a saturated aqueous picric acid solution to prevent non-specific binding of the dye to non-collagenous tissues.

    **Polarization Microscopic Studies of Connective Tissue Stained with Picro-Sirius Red FBA.**
     ***Puchtler et al. (1973).***

    >>***Summary:*** Polarization microscopic studies are usually carried out on unstained tissues. However, polarization microscopy of dyed fibers has long been used in the textile industry and observations were correlated with x-ray diffraction data. In this study the principles of polarization microscopy of stained fibers were applied to connective tissue. Human autopsy material was fixed in buffered and unbuffered formalin, Zenkerformol, Carnoy's fluid or methacarn. Deparaffinized sections were stained in a 0.1% solution of Sirius F3BA in saturated aqueous picric acid for 30 minutes, dehydrated and mounted. Sirius red F3BA enhanced the birefringence of collagen and reticulum fibers significantly. Elastin, basement membranes, ring fibers, and related structures were isotropic. Collagen fibers in various lesions, e. g., glomerular fibrosis, early arteriosclerosis, were easily identifiable by their strong birefringence. The stain was found advantageous for general pathology because it permits direct comparison of familiar staining patterns with the polarization microscopic pitcure. Correlation of polarization microscopic observations with electron microscopic and x-ray diffraction data demonstrated relations between molecular orientation of connective tissue structures and birefringence.

    >> The stain was found advantageous for general pathology because it permits direct comparison of familiar staining patterns with the **polarization** microscopic pitcure.



3. **Biological Stain Commission Standards:** The red pigment is officially identified as **Sirius Red F3B** (Generic name: **Direct Red 80**, Colour Index: **CI 35780**). It is a polyazo dye known for not releasing benzidine upon degradation, making it a safer alternative to older dyes.


### 2. Polarized Light Microscopy & 0.1% Concentration

1. **Junqueira et al. (1979):** The application of the PSR stain for evaluating collagen under polarized light was pioneered by Junqueira, Bignolas, and Brentani. Their research demonstrated that Sirius Red F3B binds parallel to the collagen fibrils, dramatically enhancing their natural birefringence.

    >> ***Summary:*** Tissue samples were embedded in paraffin, sectioned at 5 gm and stained for 1 h in the Picrosirius solution described by Sweat et al. (1964), (0.1% solution of Sirius Red F3BA in saturated aqueous picric acid: Sirius Red F3BA obtained from Verona Dyestuffs, P.O. Box 385, Springfield Road, Union, New Jersey). This solution has a pH of 2. The stained sections were then washed for 2 min in 0.01 N HCI, dehydrated, cleared and mounted in synthetic resin. A counterstain with Harris' Haematoxylin was frequently employed after the Picrosirius staining. 

    >> When serial sections were stained with Sirius Red at different pH and the stain eluted and quantitated, the results showed a peak of staining around pH 2 (Fig. 4). The concentration of picric acid is not critical, as suggested by Constantine & Mowry (1968). Thus, in skin sections, the same uptake of stain occurs in saturated picric acid as in weaker solutions (Fig. 5). Despite the fact that the concentration of picric acid is not critical for the Sirius Red-collagen interaction in the range we studied, a saturated solution should be used to avoid staining of other tissue components as referred to previously. The procedure for washing the stained sections is also important, for we observed that tap water removes the dye slowly. Thus a brief wash (2 rain) in a 0.01 N hydrochloric acid solution is recommended. The concentration of Sirius Red in the staining solution is critical. Fig. 6 shows the influence of increasing amounts of dye in the Picrosirius solution. It is apparent from the figure that the concentration of 0.1% recommended by Sweat et al. (1964) is suitable. The staining process is progressive with time, reaching saturation after 1 h as shown in Fig. 7.

2. This specific 1979 methodology is what **standardized the 0.1% concentration** (0.1 g of Sirius Red F3B in 100 mL of saturated aqueous picric acid) that is used in the vast majority of labs today.

### 3. Variations in Dye Concentration (0.01% to 0.5%)

* **Canham et al. (1999) & Stain Certification Protocols:** Research into the chemical properties and certification of Sirius Red F3B notes that while 0.1% is the standard, the dye remains effective as a collagen stain over a broad concentration range from **0.01% up to 0.5%** when dissolved in saturated aqueous picric acid.
* Concentrations at the upper limit (0.5%) approach the **saturation point of the Sirius Red in the picric acid solvent**, which can leave undissolved red material in the solution and **increase the risk of background staining**. Lower concentrations (0.01% to 0.05%) are adapted by individual laboratories for extended staining times or specialized tissue preparations.