# Task 1 - Data Cleaning and Preprocessing (Netflix Dataset)

## 1. Dataset Information
- **Dataset Name:** Netflix Movies and TV Shows  
- **Source:** Kaggle (netflix_titles.csv)  
- **Rows (Original):** 8,807  
- **Columns:** 12  

## 2. Objective
The goal of this task was to clean and preprocess the raw Netflix dataset by handling missing values, removing duplicates, standardizing text formats, fixing date formats, and ensuring correct data types so that the dataset becomes ready for analysis.

## 3. Steps Performed
1. **Trimmed and cleaned text columns** (`title`, `director`, `cast`, `country`, `listed_in`, `description`) using TRIM and CLEAN to remove extra spaces and hidden characters.  
2. **Handled missing values**:  
   - Replaced blanks in `director`, `country`, and `rating` with "Unknown".  
   - Kept missing values in `date_added` as blank since `release_year` is still available.  
3. **Removed duplicates** using a composite key (`title + release_year + type`).  
4. **Standardized categorical fields**:  
   - Ensured `type` has only two values: `Movie` and `TV Show`.  
   - Cleaned `rating` values for consistency.  
5. **Converted `date_added`** column into a uniform format: `dd-mm-yyyy`.  
6. **Renamed and checked columns/data types**:  
   - Standardized column headers to lowercase with underscores (e.g., `show_id`, `release_year`).  
   - Ensured `release_year` is numeric, `date_added` is date type, and `duration` is split into numeric + unit.# 
