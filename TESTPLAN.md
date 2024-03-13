# Test Plan for BalancedBrackets

## Test Cases

1. **Only Brackets Return True**
    - Input: "[]"
    - Expected Output: true

2. **Empty String Returns True**
    - Input: ""
    - Expected Output: true

3. **Nested Brackets Are Allowed**
    - Input: "[Launch[Code]]"
    - Expected Output: true

4. **Brackets in Correct Order Return True**
    - Input: "Launch[Code]"
    - Expected Output: true

5. **Incorrect Order Returns False**
    - Input: "[LaunchCode"
    - Expected Output: false

6. **MisnNesting Returns False**
    - Input: "Launch]Code["
    - Expected Output: false

7. **Single Bracket Returns False**
    - Input: "["
    - Expected Output: false

8. **Consecutive Brackets Returns False**
    - Input: "]["
    - Expected Output: false

9. **Non-Bracket Characters Are Allowed**
    - Input: "Launch[Code] is awesome!"
    - Expected Output: true

10. **Multiple Bracket Pairs Return True**
    - Input: "[Launch][Code]"
    - Expected Output: true

11. **Brackets With Other Characters Return True**
    - Input: "[]LaunchCode!"
    - Expected Output: true

12. **Brackets With White Space Return True**
    - Input: "[   Launch   Code   ]"
    - Expected Output: true

13. **Brackets With Mixed Characters Return False**
    - Input: "[Launch]Code[ is ]not[ balanced"
    - Expected Output: false



