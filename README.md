# Convolutional Neural Networks Seminar

A study and presentation of **DeepCSeqSite**, a deep convolutional neural network for predicting **protein–ligand binding residues directly from protein sequences**.

The seminar focuses on the motivation for using temporal convolutions, the DeepCSeqSite encoder/decoder architecture, effective context scope, optimization, evaluation, and the enhanced decoder.

## Material

* [Presentation](presentation.pdf)
* [Written Summary](Summary.pdf)
* [Outline](outline.txt)

## Primary Source

**Cui, Y., Dong, Q., Hong, D. & Wang, X.**
*Predicting protein-ligand binding residues with deep convolutional neural networks*
BMC Bioinformatics, 20, 93 (2019).

* [Research Paper — DOI](https://doi.org/10.1186/s12859-019-2672-1)
* [Full Text — PubMed Central](https://pmc.ncbi.nlm.nih.gov/articles/PMC6390579/)
* [Original DeepCSeqSite implementation and datasets](https://github.com/yfCuiFaith/DeepCSeqSite)

## Data

The paper's datasets are derived from **BioLiP**, a curated database of biologically relevant protein–ligand interactions, with protein structure information originating primarily from the Protein Data Bank.

* [BioLiP](https://zhanggroup.org/BioLiP/)
* [Protein Data Bank (PDB)](https://www.rcsb.org/)

## Core Idea

Given a protein's amino-acid sequence, predict **for every residue whether it participates in ligand binding**, using stacked 1D convolutions to build a large effective context while retaining parallel sequence processing.
