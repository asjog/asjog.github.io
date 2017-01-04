---
layout: page
title: Research
---
* <h2> Image Synthesis in Neuroimaging </h2>
Automatic processing of magnetic resonance images (MRI) is a vital part of neuroscience research. Yet even the best and most widely used medical image processing methods will not produce consistent results when their input images are acquired with different pulse sequences. The lack of consistency is a result of multiple sources of variation in the acquired MRI data. MRI, unlike computed tomography (CT), does not produce images where the magnitude of the intensity is standardized across scanners. In a typical scanning session, different MRI pulse sequences are acquired at different resolutions for various reasons. Certain pulse sequences are prone to artifacts that cause corrupted data. Image synthesis has been proposed to enhance and/or homogenize acquired MRI data. We have developed three different approaches to perform image synthesis in MRI:
  <ol>
  <li><a href="#psiclone">PSICLONE</a></li>
  <li><a href="#replica">REPLICA</a></li>
  <li><a href="#synthcraft">SynthCRAFT</a></li>
  </ol>

  - <h3 id="psiclone"> PSICLONE </h3>
    PSICLONE (<b>P</b>ulse <b>S</b>equence <b>I</b>nformation-based <b>C</b>ontrast <b>L</b>earning <b>O</b>n <b>N</b>eighborhood <b>E</b>nsembles) is an image synthesis and intensity standardization framework.
    <center>
      <img src="/images/new_psi-clone_flowchart.jpg" alt="PSICLONE" height="420" align="middle">
    </center>

    PSICLONE estimates approximate pulse sequence parameters of a given MR image to generate subject-specific training images that are used to train a random forest regression to synthesize a target contrast. The learnt regression is applied to the given image to generate a synthetic or a standardized image.

    Paper: [doi](http://dx.doi.org/10.1016/j.media.2015.05.002)

    Software: [coming soon]()

    - <h3 id="replica"> REPLICA </h3>
    REPLICA (<b>R</b>egression <b>E</b>nsembles with <b>P</b>atch <b>L</b>earning for <b>I</b>mage <b>C</b>ontrast <b>A</b>greement) is a supervised, multi-resolution image synthesis approach that uses random forests as the main regression engine. REPLICA can be used as an image synthesis approach on its own as well as a subroutine in <a href="psiclone">PSICLONE</a>.
    <center>
      <img src="/images/replica_flow_diagram.jpg" alt="REPLICA" height="420" align="middle">
    </center>
    The REPLICA can be adapted to perform example-based super-resolution of MR images as well.

    Paper: [doi]()

    Software: [coming soon]()
