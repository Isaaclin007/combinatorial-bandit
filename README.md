# Combinatorial Multi-Armed Bandit

A method for selecting a subset of best items w.r.t. black-box reward function: Given a set of 𝑁 items, the algorithm searches for an optimal 𝑠𝑢𝑏𝑠𝑒𝑡 of a maximum number of 𝑘 items, which maximizes a blackbox reward function 𝑓(𝑠𝑢𝑏𝑠𝑒𝑡).

The algorithm generates new subset candidates based on the novelty of the items while also considering what is the ratio of presence of an item that exist among the top previously tried subsets (by sorting them w.r.t. the rewards achieved).

The algorithm is not yet perfect but it just takes few thousand trials to find 4 out of 5 best items from a set of 100 items where one would need to make up to few million trials with a pure random search to achieve the same local maximum.
