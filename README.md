# Land Use Categorization of Google Earth Engine Images
Categorizing land usage based on images gathered from Google Earth Engine

Understanding and tracking changes in land use (ex. agricultural > housing) can open understanding into how humans are impacting our local ecosystems on a macro-scale.  Beyond a simple category change, these insights could be extended to take into account estimated investment and impact from supporting infrastructure (buildings generally require connection to an electrical grid, access to water and roadways) and GHG emissions using heuristics.

Google Earth Engine provides high resolution earth imagery at a wide range of zoom levels.  Though these images are updated periodically (approximately on an annual basis in some areas), they can be assumed to be a near-current snapshot.  Access to updated imagery covering the assessed areas on a fixed cadence (for example, sourced from [Planet.com](planet.com)) would enable this method to generate land use as a time series to explore trends.

### Data Sources
#### Training Data
Prediction of categories for new images requires the the model to be trained on labeled data.  The EuroSAT dataset contains 27000 georeferenced satellite images, labeled over ten land use classes:
 - AnnualCrop
 - HerbaceousVegetation
 - Industrial
 - PermanentCrop
 - River
 - Forest
 - Highway
 - Pasture
 - Residential
 - SeaLake


https://github.com/phelber/EuroSAT#
https://colab.research.google.com/drive/1nOL7rB8EnFTvLoarerVOtECYBwJKth-t?usp=sharing#scrollTo=Qw688STi6Z6k
https://zenodo.org/record/7711810#.ZAm3k-zMKEA