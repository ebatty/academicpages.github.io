---
title: "YASS: Yet Another Spike Sorter"
collection: publications
permalink: /publication/YASS
date: 2017-12-15
venue: 'NIPS'
excerpt: 'Lee, J., Carlson, D., Shokri, H., Yao, W., Goetz, G., Hagen, E., Batty, E., Chichilnisky, E., Einevoll, G.,
Paninski, L. YASS: Yet Another Spike Sorter. Advances in Neural Informational Processing Systems 2017.'

---

Abstract: Spike sorting is a critical first step in extracting neural signals from large-scale
electrophysiological data. This manuscript describes an efficient, reliable pipeline
for spike sorting on dense multi-electrode arrays (MEAs), where neural signals
appear across many electrodes and spike sorting currently represents a major
computational bottleneck. We present several new techniques that make dense MEA
spike sorting more robust and scalable. Our pipeline is based on an efficient multistage
“triage-then-cluster-then-pursuit” approach that initially extracts only clean,
high-quality waveforms from the electrophysiological time series by temporarily
skipping noisy or “collided” events (representing two neurons firing synchronously).
This is accomplished by developing a neural network detection method followed
by efficient outlier triaging. The clean waveforms are then used to infer the set
of neural spike waveform templates through nonparametric Bayesian clustering.
Our clustering approach adapts a “coreset” approach for data reduction and uses
efficient inference methods in a Dirichlet process mixture model framework to
dramatically improve the scalability and reliability of the entire pipeline. The
“triaged” waveforms are then finally recovered with matching-pursuit deconvolution
techniques. The proposed methods improve on the state-of-the-art in terms of
accuracy and stability on both real and biophysically-realistic simulated MEA data.
Furthermore, the proposed pipeline is efficient, learning templates and clustering
faster than real-time for a ' 500-electrode dataset, largely on a single CPU core.

[Code available here](https://github.com/paninski-lab/yass)

[Paper available here](http://papers.nips.cc/paper/6989-yass-yet-another-spike-sorter.pdf)

Lee, J., Carlson, D., Shokri, H., Yao, W., Goetz, G., Hagen, E., Batty, E., Chichilnisky, E., Einevoll, G.,
Paninski, L. YASS: Yet Another Spike Sorter. Advances in Neural Informational Processing Systems 2017.
