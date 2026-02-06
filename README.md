<h1 style="color:#1f4e79;">QuPath for Bone Histomorphometry</h1>

<p style="font-size:15px;">
This repository accompanies a video tutorial introducing
<strong style="color:#1f4e79;">QuPath</strong> and demonstrating its application to
<strong>bone histomorphometry</strong> using whole-slide images.
</p>

<p>
<img src="https://raw.githubusercontent.com/qupath/qupath/main/docs/images/qupath_screenshot.png"
     alt="QuPath interface showing whole-slide image"
     style="border:1px solid #ccc; border-radius:6px; width:100%;">
</p>

<hr style="border:0; border-top:2px solid #e6e6e6;">

<h2 style="color:#2f6f4e;">Why QuPath?</h2>

<p>
ImageJ has been widely used for image analysis; however, it has several limitations when working with
very large histological images. Certain file formats, such as <em>OME-TIFF</em>, are not fully supported
and may require additional conversion steps. Furthermore, large whole-slide images (e.g. VSI files)
may open at reduced resolution, resulting in loss of cellular-level detail.
</p>

<p>
To address these challenges, we adopted <strong style="color:#1f4e79;">QuPath</strong>,
which is specifically designed for efficient visualization and analysis of whole-slide images
while preserving full resolution.
</p>

<hr style="border:0; border-top:2px solid #e6e6e6;">

<h2 style="color:#2f6f4e;">About QuPath</h2>

<ul>
  <li><strong>Free and open-source</strong></li>
  <li>Available for Linux, Windows, and macOS</li>
  <li>Optimized for whole-slide image analysis</li>
  <li>Actively developed with strong community support</li>
</ul>

<p>
QuPath can smoothly handle multi-gigabyte images scanned at high magnification (e.g. 20×),
with dimensions exceeding 50,000 pixels per axis, while maintaining full cellular resolution.
</p>

<hr style="border:0; border-top:2px solid #e6e6e6;">

<h2 style="color:#2f6f4e;">Bone Histomorphometry Examples</h2>

<h3 style="color:#4f81bd;">Trabecular Bone Area and Perimeter (Von Kossa)</h3>

<p>
Following standard rodent histomorphometry guidelines, the video demonstrates how to measure
<strong>tissue area</strong>, <strong>bone area</strong>, and <strong>bone perimeter</strong>
using a Von Kossa–stained section.
</p>

<ol>
  <li>Select the cancellous bone region using brush or polygon tools</li>
  <li>Define two pixel classes:
      <span style="color:#1f4e79;"><strong>bone</strong></span> and
      <span style="color:#6b6b6b;"><strong>marrow</strong></span>
  </li>
  <li>Train a pixel classifier using representative annotations</li>
  <li>Apply morphological post-processing to refine segmentation</li>
</ol>

<p>
Post-processing steps include removing small objects (noise) and filling small holes within bone regions,
resulting in a clean and biologically meaningful bone mask.
</p>

<p>
Once trained, the classifier can be reused across multiple images or applied to the entire project.
</p>

<hr style="border:0; border-top:2px solid #e6e6e6;">

<h3 style="color:#4f81bd;">Integration with ImageJ</h3>

<p>
QuPath supports exporting selected regions to ImageJ, typically after downsampling.
In ImageJ, additional plugins such as <strong>BoneJ</strong> can be used to calculate
parameters including <em>mean trabecular thickness</em>.
</p>

<hr style="border:0; border-top:2px solid #e6e6e6;">

<h2 style="color:#2f6f4e;">Osteoclast Quantification (TRAP Staining)</h2>

<h3 style="color:#b03a2e;">Positive Cell Detection</h3>

<p>
TRAP-positive osteoclasts are identified using QuPath’s built-in
<strong>positive cell detection</strong> tool. Red-stained regions correspond to osteoclasts,
and in many cases default parameters provide reliable results.
</p>

<p>
This approach yields osteoclast counts as well as per-cell measurements
(e.g. cell area and nucleus area), which can be exported for downstream analysis.
</p>

<h3 style="color:#b03a2e;">Object Classification</h3>

<p>
An alternative strategy involves machine-learning–based
<strong>object classification</strong>.
All cells are detected first, followed by manual annotation of osteoclasts
and non-osteoclasts to train the classifier.
</p>

<p>
While effective in some cases, this approach generally requires more manual annotation
and is more sensitive to staining variability.
</p>

<hr style="border:0; border-top:2px solid #e6e6e6;">

<p style="font-style:italic; color:#555;">
Thank you for watching.
</p>
