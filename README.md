cd ~/Assignment2_EmployeeData
cat > README.md << 'EOF'
# Tutedude Assignment 2: Employee Data Processing
**Chirag Girawale | Tutedude Online Course | Data Analyst | Pune, Maharashtra | Feb 22, 2026**

---

## ✅ TASK COMPLETION STATUS (5/5 Tasks Mastered)

| Task # | Requirement | Status | Implementation Details |
|--------|-------------|--------|----------------------|
| **1** | Sort Salary descending | ✅ **COMPLETE** | E105(65K) → E104(45K), Data → Sort → Column D → Z→A |
| **2** | HR Department filter | ✅ **COMPLETE** | Filter arrows on all headers, HR shows John+Bob (2/5) |
| **3** | Split names to F/G columns | ✅ **COMPLETE** | Inserted F&G first, Text-to-Columns on copied names |
| **4** | Remove E104 duplicate | ✅ **COMPLETE** | Data → Remove Duplicates → Employee_ID column only |
| **5** | Formal table formatting | ✅ **COMPLETE** | Insert → Table + bold headers + alternating row colors |

---

## 🛠️ DETAILED CHALLENGES & PROBLEM-SOLVING DOCUMENTATION

### **Challenge 1: Name Column Splitting Overwrite Issue**
**Problem**: Standard Text-to-Columns on column B overwrote Salary (column C) data completely.  
**Root Cause**: Excel's Text-to-Columns splits data into adjacent columns without warning.  
**Solution Applied**: 
1. Inserted empty columns F and G before processing
2. Copied original Name column to F1:F6 
3. Applied Text-to-Columns **only** on column F (Space delimiter)
4. Renamed F1→"First_Name", G1→"Last_Name"
5. Deleted original column B safely  
**Time Resolved**: 12 minutes of experimentation  
**Key Learning**: Always prepare destination columns before splitting operations

### **Challenge 2: Excel Online Table Formatting Limitations**
**Problem**: Excel Online lacked "Format as Table" dropdown found in desktop version.  
**Root Cause**: Web version has reduced formatting options compared to desktop Excel.  
**Solution Applied**: Used **Insert → Table** feature instead, then manually:
1. Applied bold formatting to row 1 headers (Ctrl+B)
2. Added light grey fill to headers for visual distinction  
**Result**: Professional table appearance matching desktop Excel output  
**Key Learning**: Excel Online Insert→Table provides equivalent functionality

### **Challenge 3: Duplicate Detection Failure**
**Problem**: Excel reported "No duplicates found" despite clear E104 duplication.  
**Root Cause**: Remove Duplicates checked **all columns** instead of unique identifier.  
**Solution Applied**: 
1. Selected **Employee_ID column only** (A1:A7)
2. Data → Remove Duplicates → Employee_ID checked exclusively  
**Result**: Row 6 (duplicate E104) successfully removed, 6→5 rows  
**Key Learning**: Always use primary key (Employee_ID) for deduplication

### **Challenge 4: Filter Persistence After Sorting**
**Problem**: HR filter cleared when resorting by salary.  
**Root Cause**: Filter state not preserved during sort operations.  
**Solution Applied**: Applied final HR filter **after** all sorting completed  
**Result**: Both sorting AND filtering functional simultaneously  

---

## 📊 FINAL DATASET VALIDATION


