**# SFDX App**

**## Description of Files and Directories**

This project can be used to demonstrate picklist values not being updating in new package versions.

**Folders**

---force-app/stage1/  : This can be used to create the first package.  It contains two custom picklist fields. 

---force-app/stage2/  : This can be used to create the second package.  It contains the same custom picklist fields as stage1 with a new picklist value added

**Recreate Steps**

1. Create a new package and package version for "stage1"
2. Install package in test org.  New fields should be create with one picklist value each
3. Create a new package and package version for "stage2".  This can be achieved by chaing the package source direcoty in project.json.
4. Install new package in test org.  New values will not appear on custom picklist fileds.