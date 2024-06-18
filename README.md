# Towards Understanding Personality Expression via Body Motion
This repository contains our code and data for our work-in-progress article published in MASSXR 2024.

We label selected animation samples from two datasets:
- [Bandai-Namco-Research-Motiondataset](https://github.com/BandaiNamcoResearchInc/Bandai-Namco-Research-Motiondataset.git)
- [ZeroEGGS: Zero-shot Example-based Gesture Generation from Speech](https://github.com/ubisoft/ubisoft-laforge-ZeroEGGS.git)

The following CSV files include the personality labels by different users:
- [ZeroEGGS_Study_Results.csv](ZeroEGGS_Study_Results.csv)
- [Bandai_Study_Results.csv](Bandai_Study_Results.csv)

Our code in [animation_personality.ipynb](animation_personality.ipynb), which can work on [Google Colab](https://colab.research.google.com/), performs the following operations:
- Downloads the animation data from [Bandai](https://github.com/BandaiNamcoResearchInc/Bandai-Namco-Research-Motiondataset.git) and [ZeroEGGS](https://github.com/ubisoft/ubisoft-laforge-ZeroEGGS.git) repositories
- Prepares the ZeroEGGS subsamples using the manually marked animation clip times in [zeroeggs_subsample_times.zip](zeroeggs_subsample_times.zip)
- Calculates Laban Motion Analysis (LMA) features from ZeroEGGS subsamples for finding the 100 subsamples of unique motion features through an elimination process

```
@INPROCEEDINGS{SonluEtal2024MASSXR2024,
  author={Sinan Sonlu and Yal{\i}m Do{\^g}an and Ar{\c c}in {\"U}lk{\"u} Erg{\"u}zen and Musa Ege {\"U}nalan and Serkan Demirci and Funda Durupinar and U{\^g}ur G{\"u}d{\"u}kbay},
  booktitle={Proceedings of the IEEE Conference on Virtual Reality and 3D User Interfaces, Workshop on Multi-modal Affective and Social Behavior Analysis and Synthesis in Extended Reality}, 
  series = {MASSXR~'24},
  title={Towards Understanding Personality Expression via Body Motion}, 
  year={2024},
  pages={628-631},
  keywords={Solid modeling; Correlation; Three-dimensional displays;Costs; Conferences;Estimation; Virtual reality; Computing methodologiesâ€”Artificial intelligenceâ€”Computer visionâ€”Activity recognition and understanding; Computing methodologiesâ€”Computer graphicsâ€”Animationâ€”Motion processing},
  doi={10.1109/VRW62533.2024.00123},
  publisher = {IEEE},
  address = {Piscataway, NJ, USA},
  abstract= {This work addresses the challenge of data scarcity in personality-labeled datasets by introducing personality labels to clips from two open datasets, ZeroEGGS and Bandai, which provide diverse full-body animations. To this end, we present a user study to annotate short clips from both sets with labels based on the Five-Factor Model (FFM) of personality. We chose features informed by Laban Movement Analysis (LMA) to represent each animation. These features then guided us to select the samples of distinct motion styles to be included in the user study, obtaining high personality variance and keeping the study duration and cost viable. Using the labeled data, we then ran a correlation analysis to find features that indicate high correlation with each personality dimension. Our regression analysis results indicate that highly correlated features are promising in accurate personality estimation. We share our early findings, code, and data publicly.}
   bib2html_dl_pdf = "http://www.cs.bilkent.edu.tr/~gudukbay/publications/papers/conf_papers/Sonlu_Et_Al_MASSXR_2024.pdf",
 bib2html_pubtype = {Refereed Conference Papers},
 note = {<a href="https://ieeexplore.ieee.org/document/10536396">Publisher Web Site</a>},
 bib2html_rescat = {Computer Graphics}
}
```
