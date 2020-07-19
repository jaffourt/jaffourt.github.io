.. title: 
.. slug: optimal-adversarial-location-and-pathway-estimation
.. date: 2020-07-18 16:51:31 UTC-04:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
.. has_math: true
.. hidetitle: true
.. password: true
Optimal Adversarial Location and Pathway Estimation Using Remotely Sensed Spectral-Terrain Data: A Graphical Modeling Approach

1. First we attempt to reduce dimensionality by eliminating redundant noise in the HSI image. The primary method employed was PCA.

   .. math::
      \mathbf{T}_L = \mathbf{X} \mathbf{W}_L

   Keeping only the first :math:`L` principal components, produced by using only the first :math:`L` eigenvectors. We attempt to classify using :math:`L=7`.

2. We then attempt to reduce dimensionality by searching for a spectral dictionary of linearly independent signals using a novel algorithm ATGP, which performs an orthogonal subspace projection on the raw HSI data. ATGP attempts to define each pixel :math:`\mathbf{Y}` as the following:

   .. math::
      \mathbf{Y}=a_0 P_0+a_1 P_1+...+a_n P_n

   We then iteratively create a spectral dictionary from the most abundant spectrally distinct signals in each pixel, constrained to some number of targets :math:`T=7`. 
   
3. OC

Unfortunately the final report cannot be shared publicly, but a draft of a technical report describing these methods can be downloaded `here <https://www.josefaffourtit.com/portfolio/Affourtit_RR_2017.pdf>`__.
