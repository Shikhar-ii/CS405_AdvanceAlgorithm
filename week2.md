Gale-Shapley
Men propose in preference order.
Women keep the better proposal.
Once engaged, a woman never becomes free.
A woman's partner gets better over time.
If rejected, a man proposes to his next choice.
A rejected man never proposes to the same woman again.
The algorithm stops when everyone is matched.
Men move down their list; women move up their list.
Matching

A matching is a set of pairs where each person has at most one partner.

Example:

m1 ↔ w2
m2 ↔ w1
m3 ↔ w3
Stable Matching

A stable matching has no blocking pair.

A blocking pair is a man and woman who:
Think of it like this:

1. IF

If it rains, then the ground is wet.

Rain → Wet

Only one direction.

2. ONLY IF

The ground is wet only if it rains.

Wet → Rain

Still one direction, but the direction is reversed.

3. IF AND ONLY IF (IFF)

The ground is wet if and only if it rains.

Rain ↔ Wet

Both directions.

Easy trick
A if B → B → A
A only if B → A → B
A iff B → A ↔ B

are not matched together, and
both prefer each other over their current partners.
Remember

Matching: Everyone has a partner.
Stable matching: No two people want to switch partners


During the Algorithm

A man can be free if he has not proposed to all women yet.

So:

Free man + women left to propose to
        ↓
Propose to his next choice

The algorithm continues while there is a free man who has not proposed to every woman.

Remember

Free man + someone left → propose.

If a man is free and has already proposed to every woman, the algorithm cannot continue with him.

