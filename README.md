# Install Autopsy and Analyze the Disk File and Folder Configuration
# Lubindher S
# 212222240056

## AIM
To install **Autopsy** and use it to analyze the disk’s file and folder configuration for forensic investigation.

## REQUIREMENTS
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tools**:  
  - [Autopsy Digital Forensics Platform](https://www.autopsy.com/)  
  - Optional: Sleuth Kit CLI tools for deeper analysis
- **Test Data**: Disk image file (`.dd`, `.img`, `.E01`)

## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Install Autopsy]
    B --> C[Create New Case in Autopsy]
    C --> D[Add Data Source: Disk Image]
    D --> E["Autopsy Modules Run: File System, Metadata, Keywords"]
    E --> F[File & Folder Structure View]
    F --> G[Export / Recover Files]
```
## DESIGN STEPS:
### Step 1:
Download Autopsy from the official website and install it on your system.

### Step 2:
Launch Autopsy and create a new case.

### Step 3:
Add your disk image or physical drive as the data source.

### Step 4:
Allow Autopsy to run its built-in ingest modules (file system analysis, hash lookup, keyword search, metadata extraction).

### Step 5:
View the file and folder hierarchy in the left-hand tree panel.

### Step 6:
Export or recover files if required for the investigation.

## PROGRAM(Windows)

1. Download Autopsy from autopsy.com.
2. Install and launch the application.
3. Select **New Case → Name your case → Choose case folder**.
4. Click Add **Data Source → Select Disk Image → Browse to file**.
5. Choose ingest modules (file system, metadata, hash lookup, keyword search).
6. Wait for processing to finish.
7. Explore file/folder structure in the navigation pane.
8.Export selected files for further examination.

## OUTPUT:
File and Folder Configuration Analysis Results
<img width="1894" height="984" alt="Screenshot 2025-09-07 101955" src="https://github.com/user-attachments/assets/05dc0746-8ec3-4f36-9dd1-e7c07fe4acbf" />
<img width="1920" height="1080" alt="Screenshot 2025-09-07 100629" src="https://github.com/user-attachments/assets/3116ee97-7c76-4545-b28d-50425ce425c2" />
<img width="981" height="574" alt="Screenshot 2025-09-07 102029" src="https://github.com/user-attachments/assets/28fd25a6-2d14-4af2-8794-0809cc6528b1" />
<img width="1908" height="1008" alt="Screenshot 2025-09-07 101702" src="https://github.com/user-attachments/assets/1ee56f72-2221-4ca4-8814-3a7ee9334d98" />
<img width="1920" height="1080" alt="Screenshot 2025-09-07 101852" src="https://github.com/user-attachments/assets/f4419d64-b7dd-4a40-9a5d-e3d15bb8ccf4" />

## RESULT:
Autopsy was installed successfully and used to analyze disk, file, and folder configuration for forensic investigation.
