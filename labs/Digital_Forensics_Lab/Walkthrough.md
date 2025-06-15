# Digital Forensics Lab Walkthrough

## Course: Management of Information Security

### Lab: Understanding the Digital Forensics Profession and Investigations

---

## Introduction

This lab develops hands-on skills in:

* Acquiring an Image of Evidence Media
* Analyzing Digital Evidence
* Generating Reports and Keyword Searches

**Estimated Lab Time**: \~1 hour

**Exam Objectives**:

* Prepare a forensic toolkit and use appropriate tools
* Recommend remediation strategies based on forensic analysis

---

## Lab Setup

You will be working on the **Windows 8.1 Workstation**. Start the device and open **ProDiscover Basic 64** as an Administrator.

---

## Exercise 1 - Acquiring an Image of Evidence Media

### Objective

Use **ProDiscover Basic** to acquire an image from a USB drive (Drive E:).

### Steps

1. Navigate to `C:\Work`.
2. Launch ProDiscover Basic 64 as Administrator.
3. Go to `Action > Capture Image`.
4. Select Drive `E:` as source.
5. Save the image in `C:\Work\Data files\Ch01` as `InChp01-prac`.
6. Enter technician name and image number `InChp01-prac01`.
7. Wait for acquisition to complete. Save log file and note MD5 hash.
8. Exit ProDiscover Basic.

**📸 Screenshot:** Acquisition completion message box

---

## Exercise 2 - Analyzing Your Digital Evidence

### Task 1: Load Acquired Image

1. Start a new project: `InChp01`
2. Add the image: `InChp01-prac.eve`
3. View the image under `Content View > Images`

### Task 2: Keyword Search

1. Open `Search > Content Search`
2. Search for keyword: `plabwin810`
3. View results under `Search Results > tracking.log`

**📸 Screenshot:** Search result showing `plabwin810`

### Task 3: Report Creation

1. Click `Report` in tree view.
2. Print to Microsoft XPS Document Writer as `Ch01-Report`
3. View report using `XPS Viewer`

### Task 4: Export Report

1. Reopen ProDiscover project
2. Export report as `.RTF` file: `InChp01.rtf`
3. Open in OpenOffice Writer

---

## Exercise 3 - Analysis Example

### Objective

Identify key evidence by searching for keywords such as `fragment` and `1cro`.

### Tasks

* Start project `C1Prj02`
* Load image: `FATSearchTestImage.eve`
* Perform keyword search for `fragment`
* Export search report as `Ch1Prj02Report`

### Additional Keyword Search

* New project: `C1Prj03`
* Search for: `1cro`
* View images in Gallery View

**📸 Screenshot:** Search results for `fragment` and `1cro`

---

## Exercise 4 - Allocated & Unallocated Files

### Task 1: Allocated Data Extraction

* Create project: `C1Prj04`
* Load `PhysicalDrive1`
* Sort files by `Deleted` column
* Copy files with `Deleted: NO`

### Task 2: Unallocated File Reporting

* Create project: `C1Prj04`
* Select deleted files
* Add meaningful `Investigator Comments`
* Export report as `C1Prj05Report`

**📸 Screenshot:** Sorted files by deleted status

---

## Exercise 5 - Keyword Search Example

### Task: Perform multi-keyword search

1. Start project
2. Load `PhysicalDrive1`
3. Search keywords:

   * `plabwin810`
   * `shell`
4. Review and comment on interesting results
5. Export report

**📸 Screenshot:** Keyword search results

---

## Summary

Throughout this lab, we covered:

* Image acquisition and MD5 validation
* Analyzing active and deleted data
* Using keyword search for forensic relevance
* Creating and exporting reports in `.RTF` and `.XPS` formats

All screenshots should be saved in `/screenshots/`, and exported reports in `/reports/` folders for GitHub.

---

## Resources

* Whitman, M. E., & Mattord, H. J. (2018). *Management of Information Security* (6th ed.). Cengage Learning. ISBN: 9781337685672
