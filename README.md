# Longest Common Prefix - Three Methods

# 1. Vertical Scanning
  - Compare characters column by column across all strings
  - Stop when a mismatch is found
  - Time Complexity: O(N * M)
  - Space Complexity: O(1)
  - Best Use Case: Many strings, short length
  - Example: ["flower","flow","flight"] → "fl"

# 2. Horizontal Scanning
  - Start with the first string as the prefix
  - Compare it with each other string
  - If mismatch, shrink the prefix until it matches
  - Time Complexity: O(N * M)
  - Space Complexity: O(1)
  - Best Use Case: Balanced, easy to code, good for typical LeetCode constraints
  - Example: ["flower","flow","flight"] → "fl"

# 3. Sorting Trick
  - Sort the list of strings alphabetically
  - Compare only the first and last string
  - Their common prefix is the answer
  - Time Complexity: O(N log N + M)
  - Space Complexity: O(1)
  - Best Use Case: Moderate number of strings, long strings, concise solution
  - Example: ["flower","flow","flight"] → "fl"

# Quick Comparison:
 Vertical Scanning   → Simple, good for many short strings
 Horizontal Scanning → Balanced, easy to implement, best for LeetCode
 Sorting Trick       → Clever shortcut, but sorting adds overhead
