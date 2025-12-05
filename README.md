# PatternChroma-41K: A Large-Scale Annotated Benchmark for Color-Emotion Analysis in Visual Patterns

## Dataset Overview

PatternChroma-41K is a comprehensive dataset containing detailed color and emotional analysis of 41,015 pattern images, providing a standardized benchmark for computational design, color psychology, affective computing, and pattern recognition applications.

**Version:** 1.0  
**Total Images:** 41,015  
**Metadata Format:** JSON  

---

## Dataset Description

Each pattern image in the dataset has been analyzed using automated color extraction and emotion classification algorithms. The dataset includes:

- **Dominant color analysis** (RGB, Hex)
- **Color palettes** (6 colors per image)
- **Dimensional metadata** (width, height, aspect ratio, orientation, resolution)
- **Color metrics** (brightness, saturation, contrast)
- **Emotion classification** (12 categories)
- **Contextual tags** (111 unique descriptors)

---

## Data Structure

The metadata is provided as a JSON file with the following schema:

```json
{
  "images": [
    {
      "filename": "example.jpg",
      "path": "dataset_images/example.jpg",
      "dimensions": {
        "width": 200,
        "height": 200,
        "orientation": "Square",
      },
      "dominant_color": {
        "rgb": [120, 150, 200],
        "hex": "#7896c8"
      },
      "palette": [
        {"rgb": [120, 150, 200], "hex": "#7896c8"},
        ...
      ],
      "color_name": "BLUE",
      "brightness": 0.506,
      "saturation": 0.491,
      "contrast": 0.153,
      "emotion": "Trust",
      "contextual": "Serene"
    }
  ]
}
```

---

## Summary Statistics

### Color Features

| Feature     | N      | Mean   | SD     | Min    | Max    |
|-------------|--------|--------|--------|--------|--------|
| Brightness  | 41,015 | 0.5014 | 0.2002 | 0.0000 | 0.9978 |
| Saturation  | 41,015 | 0.4793 | 0.2334 | 0.0000 | 1.0000 |
| Contrast    | 41,015 | 0.1581 | 0.0782 | 0.0000 | 0.4977 |

### Brightness Distribution
- **Bright (>0.7):** 7,458 images (18.18%)
- **Medium (0.3-0.7):** 26,309 images (64.14%)
- **Dark (<0.3):** 7,248 images (17.67%)

### Saturation Distribution
- **High (>0.6):** 13,118 images (31.98%)
- **Medium (0.3-0.6):** 17,416 images (42.46%)
- **Low (<0.3):** 10,481 images (25.55%)

---

## Categorical Distributions

### Color Names (12 Categories)

| Color     | Count  | Percentage | 95% CI           |
|-----------|--------|------------|------------------|
| BLUE      | 7,357  | 17.94%     | [17.57%, 18.31%] |
| PURPLE    | 5,824  | 14.20%     | [13.86%, 14.54%] |
| ORANGE    | 5,156  | 12.57%     | [12.25%, 12.89%] |
| GRAY      | 3,467  | 8.45%      | [8.18%, 8.72%]   |
| YELLOW    | 3,260  | 7.95%      | [7.69%, 8.21%]   |
| RED       | 3,182  | 7.76%      | [7.50%, 8.02%]   |
| GREEN     | 3,163  | 7.71%      | [7.45%, 7.97%]   |
| TURQUOISE | 2,804  | 6.84%      | [6.59%, 7.08%]   |
| WHITE     | 2,649  | 6.46%      | [6.22%, 6.70%]   |
| PINK      | 2,586  | 6.31%      | [6.07%, 6.54%]   |
| BROWN     | 1,127  | 2.75%      | [2.59%, 2.91%]   |
| BLACK     | 440    | 1.07%      | [0.97%, 1.17%]   |

### Emotion Categories (12 Types)

| Emotion      | Count  | Percentage | 95% CI           |
|--------------|--------|------------|------------------|
| Comfort      | 6,934  | 16.91%     | [16.54%, 17.27%] |
| Imagination  | 6,676  | 16.28%     | [15.92%, 16.63%] |
| Calm         | 5,045  | 12.30%     | [11.98%, 12.62%] |
| Sadness      | 4,700  | 11.46%     | [11.15%, 11.77%] |
| Energy       | 3,795  | 9.25%      | [8.97%, 9.53%]   |
| Peace        | 3,752  | 9.15%      | [8.87%, 9.43%]   |
| Trust        | 2,792  | 6.81%      | [6.56%, 7.05%]   |
| Love         | 2,426  | 5.91%      | [5.69%, 6.14%]   |
| Balance      | 2,214  | 5.40%      | [5.18%, 5.62%]   |
| Anger        | 1,692  | 4.13%      | [3.93%, 4.32%]   |
| Joy          | 735    | 1.79%      | [1.66%, 1.92%]   |
| Fear         | 254    | 0.62%      | [0.54%, 0.70%]   |

### Top 15 Contextual Tags (111 Total)

| Context      | Count | Percentage |
|--------------|-------|------------|
| Dreamy       | 4,340 | 10.58%     |
| Melancholic  | 2,728 | 6.65%      |
| Warm         | 2,203 | 5.37%      |
| Cozy         | 2,157 | 5.26%      |
| Serene       | 2,068 | 5.04%      |
| Soft         | 1,746 | 4.26%      |
| Vibrant      | 1,678 | 4.09%      |
| Peaceful     | 1,638 | 3.99%      |
| Tranquil     | 1,236 | 3.01%      |
| Romantic     | 1,075 | 2.62%      |
| Refreshing   | 984   | 2.40%      |
| Intense      | 955   | 2.33%      |
| Passionate   | 878   | 2.14%      |
| Natural      | 840   | 2.05%      |
| Earthy       | 798   | 1.95%      |

---

## Use Cases

This dataset is suitable for:

1. **Computational Design Research**
   - Pattern classification and generation
   - Color palette extraction and recommendation
   - Design trend analysis
   - Automated pattern curation

2. **Color Psychology Studies**
   - Emotional response to color patterns
   - Color preference in decorative designs
   - Cross-cultural pattern perception
   - Affective computing in design

3. **Machine Learning Applications**
   - Training emotion recognition models
   - Pattern-based image retrieval
   - Generative design systems
   - Style transfer for patterns

4. **Textile and Fashion Research**
   - Analyzing pattern trends
   - Mood board generation
   - Seasonal color forecasting
   - Consumer preference modeling

5. **Digital Humanities and Visual Culture**
   - Pattern usage across time periods
   - Cultural pattern analysis
   - Aesthetic pattern recognition
   - Design history studies

---

## File Information

### Main Files
1. **Metadata.json**
   - Complete analysis results for all 41,015 images
   - Size: ~54.7 MB
   - Encoding: UTF-8
   - Format: JSON (JavaScript Object Notation)

2. **dataset_images.zip**
   - Complete collection of 41,015 pattern images
   - Size: ~1.9 GB (compressed)
   - Supported formats: PNG, JPG, JPEG, BMP, WEBP
   - Directory structure: `dataset_images/[filename]`

### Total Dataset Size
- **Compressed:** ~1.9 GB (ZIP archive)
- **Uncompressed:** [Specify if known]
- **Total files:** 41,016 (41,015 images + 1 JSON)

---

## Quick Start

### Using the Dataset

1. **Download the files:**
   ```bash
   # Download from Zenodo
   wget https://zenodo.org/record/17803271/files/Metadata.json
   wget https://zenodo.org/record/17803271/files/dataset_images.zip
   ```

2. **Extract the images:**
   ```bash
   unzip dataset_images.zip
   ```

3. **Load and explore the data:**
   ```python
   import json
   from PIL import Image
   
   # Load the dataset
   with open('Metadata.json', 'r') as f:
       data = json.load(f)
   
   # Access image metadata
   first_image = data['images'][0]
   print(f"Filename: {first_image['filename']}")
   print(f"Emotion: {first_image['emotion']}")
   print(f"Dominant Color: {first_image['color_name']}")
   print(f"Dimensions: {first_image['dimensions']['width']}x{first_image['dimensions']['height']}")
   
   # Load corresponding image
   img = Image.open(first_image['path'])
   img.show()
   ```

4. **Filter by emotion:**
   ```python
   # Find all "Calm" images
   calm_images = [img for img in data['images'] if img['emotion'] == 'Calm']
   print(f"Found {len(calm_images)} calm images")
   ```

5. **Filter by color:**
   ```python
   # Find all blue images with high brightness
   blue_bright = [img for img in data['images'] 
                  if img['color_name'] == 'BLUE' and img['brightness'] > 0.7]
   ```

---

## Citation

If you use this dataset in your research, please cite:

```
Boukdir, A. (2025). PatternChroma-41K: A Large-Scale Annotated Benchmark for Color-Emotion Analysis in Visual Patterns (1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.17803271
```

---

## Changelog

### Version 1.0 (2025)
- Initial release
- 41,015 images analyzed
- 12 color categories, 12 emotions, 111 contextual tags
- Added dimensional metadata
