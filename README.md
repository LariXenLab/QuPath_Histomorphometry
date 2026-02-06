<h1 style="color:#0b3c5d;">🦴 QuPath for Bone Histomorphometry</h1>

<p style="font-size:15px;">
This repository accompanies a video tutorial introducing
<strong style="color:#1f77b4;">QuPath</strong> for
<strong style="color:#2e7d32;">bone histomorphometry</strong> using whole-slide images.
All analyses shown in the video were performed at the
<strong>Ludwig Boltzmann Institute of Osteology</strong>, PL4 Group.
</p>

<div style="background:#f5f9fc; padding:10px; border-left:5px solid #1f77b4; border-radius:6px;">
<p style="margin:0;">
📹 The video explains why QuPath is needed, introduces its interface, and demonstrates
bone and osteoclast quantification workflows.
</p>
</div>

<br>



<hr style="border:0; border-top:3px solid #e0e0e0;">

<h2 style="color:#2e7d32;">🔍 Why QuPath?</h2>

<div style="background:#f1f8f4; padding:10px; border-radius:6px;">
<p>
While <strong>ImageJ</strong> is widely used, it has limitations for very large histology images,
including incomplete support for formats such as <em>OME-TIFF</em> and reduced resolution for
whole-slide images.
</p>
<p>
<strong style="color:#1f77b4;">QuPath</strong> is specifically designed to handle multi-gigabyte
whole-slide images while preserving full cellular resolution.
</p>
</div>

<hr style="border:0; border-top:3px solid #e0e0e0;">

<h2 style="color:#2e7d32;">🧪 Bone Histomorphometry</h2>

<h3 style="color:#6a1b9a;">Trabecular Bone (Von Kossa)</h3>

<div style="background:#f7f2fb; padding:10px; border-radius:6px;">
<ul>
  <li>Selection of cancellous bone regions</li>
  <li>Pixel classification into <strong style="color:#1f77b4;">bone</strong> and marrow</li>
  <li>Morphological cleanup for biologically meaningful segmentation</li>
</ul>
<p>
Bone area and perimeter are obtained directly, and trained classifiers can be reused
across images or entire projects.
</p>
</div>

<h3 style="color:#1565c0;">ImageJ Integration</h3>

<div style="background:#eef6fd; padding:10px; border-radius:6px;">
<p>
Selected regions can be exported to <strong>ImageJ</strong>, where plugins such as
<strong>BoneJ</strong> are used to calculate parameters like mean trabecular thickness.
</p>
</div>

<hr style="border:0; border-top:3px solid #e0e0e0;">

<h2 style="color:#c62828;">🩸 Osteoclast Quantification (TRAP)</h2>

<div style="background:#fdecea; padding:10px; border-radius:6px;">
<p>
TRAP-positive osteoclasts are detected using QuPath’s built-in
<strong>positive cell detection</strong> or a machine-learning–based
<strong>object classification</strong> approach.
</p>
<p>
Both methods provide osteoclast counts and per-cell measurements for downstream analysis.
</p>
</div>

<hr style="border:0; border-top:3px solid #e0e0e0;">

<p style="text-align:center; font-style:italic; color:#555;">
Thank you for watching.
</p>
