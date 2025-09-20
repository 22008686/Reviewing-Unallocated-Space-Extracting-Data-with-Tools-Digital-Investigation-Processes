![WhatsApp Image 2025-09-20 at 16 24 04_4e516735](https://github.com/user-attachments/assets/78e6e44b-a454-4a14-9a0b-1a03cf4d7b78)# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
<img width="1920" height="1080" alt="Screenshot 2025-09-20 160354" src="https://github.com/user-attachments/assets/71ad99b6-8462-494d-8ff0-e3da020c7ec5" />
<img width="1920" height="1080" alt="Screenshot 2025-09-20 160423" src="https://github.com/user-attachments/assets/b1c02813-fa77-47a9-9be1-ba97ff0dba88" />
![WhatsApp Image 2025-09-20 at 16 24 04_4e516735](https://github.com/user-attachments/assets/0295f6fe-8018-4134-b6d1-a87f90c3a931)
![WhatsApp Image 2025-09-20 at 16 24 04_6954d9e4](https://github.com/user-attachments/assets/f1aeb4ba-ab22-462b-a438-d03088c7c1d9)
![WhatsApp Image 2025-09-20 at 16 24 04_367b0263](https://github.com/user-attachments/assets/ab5c26ad-e9bf-452b-aa5d-d957cf2a897d)



Unallocated Space Analysis and Extracted Data Report

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

