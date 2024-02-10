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
