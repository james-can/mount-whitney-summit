imagery# mount-whitney-summit
Repository to store dataset captured at Whitney summit

---

## Overview
Captured using the LOOQ qCam mobile reality capture system at the summit of Mount Whitney, this dataset offers a detailed 3D look at both the highest summit as well as the highest standing structure in the contiguous US. 

* **Capture Hardware:** LOOQ qCam
* **Coordinate Reference System:** EPSG:10914 (CSRN2025 / NAD83 2011, California Zone 4, US Survey Feet)
* **Location:** Mount Whitney Summit, California

---

## Repository & File Structure

The data is organized into raw assets, processing reports, imagery, and cleanly separated component layers:

```
├── mt_whitney_summit_raw.laz         # Full-density raw point cloud
├── mt_whitney_summit_raw_thinned.laz # Raw thinned point cloud for rapid visualization
├── ppk_report.pdf                    # PPK processing report
├── imagery.geojson                   # Spatial geotags matching the panorama set
├── imagery/                          # Folder containing ground panoramas
└── mt_whitney_summit_cleaned/        # Processed and segmented working files
    ├── whitney-summit.las            # Combined cleaned point cloud asset
    └── layers/                       # Individual component layers
        ├── Shelter.laz               
        ├── Room.laz                  
        ├── Ground.laz                
        ├── Plaque.laz                
        └── Disks.laz                 
