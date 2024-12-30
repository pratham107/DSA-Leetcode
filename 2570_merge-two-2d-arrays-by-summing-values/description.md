# Merge Two 2D Arrays by Summing Values

## Problem Statement
Given two 2D integer arrays `nums1` and `nums2`, merge them into a single array while summing values for common IDs.

### Details
- Each array contains pairs `[id, value]`
- Arrays are sorted by ID in ascending order
- Each array has unique IDs
- Need to merge considering following rules:
    - Include IDs that appear in either array
    - Each ID should appear once
    - Value should be sum of values from both arrays
    - If ID missing in one array, consider its value as 0

## Examples

### Example 1
```
Input: nums1 = [[1,2],[2,3],[4,5]], nums2 = [[1,4],[3,2],[4,1]]
Output: [[1,6],[2,3],[3,2],[4,6]]
```

### Example 2
```
Input: nums1 = [[2,4],[3,6],[5,5]], nums2 = [[1,3],[4,3]]
Output: [[1,3],[2,4],[3,6],[4,3],[5,5]]
```

## Constraints
- `1 <= nums1.length, nums2.length <= 200`
- `nums1[i].length == nums2[j].length == 2`
- `1 <= idi, vali <= 1000`
- Both arrays have unique IDs
- Both arrays are sorted in ascending order by ID