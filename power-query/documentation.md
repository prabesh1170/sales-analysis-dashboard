
# Power Query Steps — Sales Data

1. Loaded tbl_SalesData into Power Query
2. Verified column quality (100% valid, no blanks/errors) using full dataset profiling
3. Removed duplicates on order_id (0 removed — confirms uniqueness)
4. Filtered Year between 2022–2026 (scope decision — excluded 2027–2035 for a realistic recent time frame)
5. Merged tbl_SalesData with tbl_RegionInfo on the 'region' column (Left Outer join)
6. Expanded regioninfo
7. Verified merge: 4 distinct managers, 0 blank values — confirms complete, correct match
