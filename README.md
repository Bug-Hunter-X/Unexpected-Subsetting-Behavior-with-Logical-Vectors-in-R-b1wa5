This repository demonstrates a subtle but potentially problematic behavior in R related to subsetting data frames using logical vectors. When a logical vector used for subsetting is longer than the number of rows in the data frame, R silently truncates the extra elements.  This can lead to incorrect results without generating any warnings or errors. The `bug.R` file showcases this issue, while `bugSolution.R` provides a solution to prevent this problem.  This is a particularly hard-to-detect error as it produces no errors or warnings.  This is important to avoid in production code.