# Histology-Testing-Silk-Worm
Oil Red O Fat Quantification ToolCore Functionality 

This Python-based image analysis tool uses OpenCV and the HSV (Hue, Saturation, Value) color space to detect and measure fat bodies in silkworm samples. It is specifically tuned to differentiate between vibrant Oil Red O stains (fat) and the natural tan or brownish-yellow background of the silkworm cuticle and internal tissues.Key FeaturesWorm Segmentation: Automatically isolates the biological sample from the white background to establish a consistent "Total Area" denominator.
High-Sensitivity Color Isolation: Uses a specific Hue range (10-20) and a high Saturation threshold (130) to lock onto the intense orange-red pixels characteristic of Oil Red O.

Quantitative Metrics: Calculates Fat Percentage, Mean Saturation (stain intensity), and Worm Area, outputting these to a tab-delimited text report for statistical analysis.

Comparative Visualization: Generates side-by-side plots of the original image and a binary "Red-on-Yellow" mask, allowing for easy verification of detection accuracy across different experimental groups (e.g., Fasting vs. Baseline).

Noise Reduction: Implements morphological "opening" operations to remove single-pixel artifacts or camera noise, ensuring only true fat body clusters are counted.

Technical StackLanguage: 
PythonLibraries: OpenCV (Image processing), NumPy (Mathematical calculations), Matplotlib (Visualization), PIL (Image handling).
