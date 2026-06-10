OITem Pillar Tracker

OITem Pillar Tracker is a browser-based video analysis tool for tracking the displacement of PDMS pillars in artificial skeletal muscle contraction experiments.

The software tracks a user-defined pillar tip using:

* Template Matching
* Local Adaptive Thresholding (Otsu)
* Contour Detection
* Minimum Enclosing Circle Fitting

The centroid position of the detected pillar tip is exported as a CSV file for subsequent force analysis.

Features

* Browser-based (no installation required)
* Circle ROI and Rectangle ROI support
* Interactive ROI creation, movement, and resizing
* ROI condition export/import via CSV
* Automatic pillar tip tracking
* Centroid coordinate export (CSV)
* Overlay video generation and preview
* Trajectory visualization
* Automatic FPS estimation
* Compatible with GitHub Pages

Tracking Workflow

1. Upload a video file
2. Display the first frame
3. Define the pillar tip ROI
4. Start tracking
5. Export tracking results as CSV
6. (Optional) Generate an overlay video

Tracking Algorithm

For each frame:

1. Template matching is performed around the previous ROI position.
2. A local search region is extracted.
3. Otsu thresholding is applied.
4. Contours are detected.
5. The largest contour is selected.
6. A minimum enclosing circle is fitted.
7. The circle center is recorded as the pillar position.

CSV Output

The exported CSV contains:

* Frame number
* Time
* X coordinate (px)
* Y coordinate (px)
* Relative displacement (dx, dy)
* Template matching score
* Fitted circle radius
* ROI parameters
* Tracking settings

Applications

* Artificial skeletal muscle contraction analysis
* PDMS pillar displacement measurement
* Tissue engineering research
* Biomechanics experiments
* Time-series motion tracking

License

MIT License

Author

Sho Yokoyama
Department of Mechanical Engineering
Osaka Institute of Technology
