# Copilot Instructions – LeetCode Workspace

Repository purpose:
This repository is used to practice LeetCode problems and data structures/algorithms locally in VSCode.

Primary language:
Python 3

Structure:
- problems/ -> one file per problem (e.g. two_sum.py, binary_tree_level_order.py)
- tests/ -> optional pytest tests
- snippets/ -> reusable helpers or data structures

Run:
python problems/<file>.py

Test (if tests exist):
python -m pytest

Build:
None (scripts only)

Lint/format (optional):
ruff check .
black .

Conventions:
- One problem per file
- Class name usually `Solution` to match LeetCode
- Prefer clean, readable solutions over clever tricks
- Add a small main block with sample inputs for quick local testing

Example template:

```python
class Solution:
    def twoSum(self, nums, target):
        pass


if __name__ == "__main__":
    s = Solution()
    print(s.twoSum([2,7,11,15], 9))

```
Agent behavior:

- Do not create complex project structure
- Keep solutions self-contained
- Prefer O(n) or optimal solutions when possible
- Add comments explaining time/space complexity