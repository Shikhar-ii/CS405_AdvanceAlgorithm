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
