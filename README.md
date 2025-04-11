# iqtree3ForkTests
This repository contains tests of [my IQ-TREE 3 branch](https://github.com/HS6986/iqtree3Fork/tree/feature/HS6986/extend-MixtureFinder) whose MixtureFinder ([Ren et al., 2024](https://doi.org/10.1093/molbev/msae264)) was extended to codon, binary, multistate, and amino acid data. See [the pull request](https://github.com/iqtree/iqtree3/pull/11) for details.

## Files
- Yamasaki2015.18S28S.Subsampled.fas: A subsample of the dataset of [Yamasaki et al. (2015)](https://doi.org/10.1186/s40851-015-0017-0) consisting of 18S and 28S rRNA sequences. It was used for the test of the DNA MixtureFinder.
- Yamasaki2015.18S28S.RY.Subsampled.fas: An RY recoded (e.g., [Braun & Kimball, 2021](https://doi.org/10.3390/birds2010001)) subsample of the dataset of [Yamasaki et al. (2015)](https://doi.org/10.1186/s40851-015-0017-0) consisting of 18S and 28S rRNA sequences. It was used for the test of the binary MixtureFinder.
- Khalturin2022.WoGaps.Subsampled.fasta: A subsample of the gapless phylogenomic dataset of [Khalturin et al. (2022)](https://doi.org/10.1126/sciadv.abo4400). It was used for the test of the amino acid MixtureFinder.
- Khalturin2022.WoGaps.recSR4.Subsampled.fasta: An SR4 ([Susko & Roger, 2007](https://doi.org/10.1093/molbev/msm144)) recoded subsample of the gapless phylogenomic dataset of [Khalturin et al. (2022)](https://doi.org/10.1126/sciadv.abo4400). It was used for the tests of the multistate MixtureFinder and my branch's behavior for multistate datasets.
- Sorensen2006.H3.Aligned.NT.Subsampled.fas; A subsample of the histone H3 alignment of [Sørensen et al. (2006)](https://doi.org/10.1111/j.1096-0031.2006.00085.x). The dataset was aligned by MACSE v2.07 ([Ranwez et al., 2018](https://doi.org/10.1093/molbev/msy159)) to account for the codon structure. The dataset was used for the test of the codon MixtureFinder.  
**This test failed with an error message `Frequency mixture name not found U`.**

## Folders
- MixtureFinder: Tests of MixtureFinder for various data types.
- Multistate: A test of my branch's behavior for multistate datasets.
