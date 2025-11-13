# Image Metadata Checker

A Python script for validating image metadata in JPEG files. This tool checks whether images contain GPS coordinates (latitude, longitude, altitude), full camera orientation data (roll, pitch, yaw), and sensor specifications (make, model, focal length, sensor width). The script parses EXIF and XMP metadata structures using only Python standard libraries, making it suitable for environments where external dependencies are not available. Results are exported to a CSV file with true/false flags for each metadata category, allowing users to identify which images in a collection meet specific metadata requirements for photogrammetry, mapping, or other geospatial applications.

## Usage

Set the `IMAGE_FOLDER` variable at the top of the script to point to your image directory, then run:

```bash
python cameraMetadataChecker.py
```

The script will generate `image_metadata_check.csv` in the specified folder with columns for image name, path, and boolean values indicating the presence of GPS coordinates, camera orientation, and sensor information.

## Requirements

- Python 3.x (standard library only)
