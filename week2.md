# Gale-Shapley & Stable Matching

## Gale-Shapley Algorithm

- Men propose in **preference order**.
- Women keep the **better proposal**.
- Once engaged, a woman **never becomes free**.
- A woman's partner gets **better over time**.
- If rejected, a man proposes to his **next choice**.
- A man never proposes to the same woman twice.
- **Men move down** their list.
- **Women move up** their list.
- The algorithm ends when **everyone is matched**.

### During the Algorithm

A man can be free if he still has women to propose to.

```text
Free man + woman left
        ↓
Propose to next choice

Remember:
Free man + someone left → Propose

Matching

A matching is a set of pairs where each person has at most one partner.

Example:

m1 ↔ w2
m2 ↔ w1
m3 ↔ w3

Remember:
Matching = people are paired.

Stable Matching

A stable matching has no blocking pair.

A blocking pair is a man and woman who:

are not matched together, and
both prefer each other over their current partners.

Remember:
Stable matching = no two people want to switch partners.

If, Only If, IFF
If
A if B
B → A
Only If
A only if B
A → B
If and Only If (IFF)
A iff B
A ↔ B

Remember:

If = one direction
Only if = one direction
IFF = both directions
For the md file GitHub workflow, one secrets-scanning option exists.
Ad


### During the Algorithm

A man can be **free** if he still has women left to propose to.

```text
Free man + women left
        ↓
Propose to next choice

The algorithm continues while there is a free man who has not proposed to every woman.

Remember

Free man + someone left → Propose

If a man is free and has already proposed to every woman, he cannot propose anymore.


Conclusion

No blocking pair can exist.

Therefore, Gale-Shapley always produces a stable matching.

Remember
m prefers w → m must have proposed to w.
w rejects m → w has someone she prefers.
w's partner only gets better.
Therefore, no blocking pair → stable matching.


Insertion sort
InsertionSort(A):
    for i = 1 to length(A) - 1:
        key = A[i]
        j = i - 1
        
        // Move elements of A[0..i-1] that are greater than key
        // to one position ahead of their current position
        while j >= 0 and A[j] > key:
            A[j + 1] = A[j]
            j = j - 1
            
        A[j + 1] = key
