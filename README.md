# leetcode-319-bulb-switcher
A C++ solution for LeetCode 319 - Bulb Switcher using the mathematical observation that only perfect square numbered bulbs remain ON after all rounds.
Problem

There are n bulbs initially off. After performing n rounds of toggling, determine how many bulbs remain on.

Approach

Each bulb is toggled once for every divisor of its position number.

Numbers usually have divisors in pairs.
Perfect squares have one unpaired divisor.
Therefore, only bulbs at perfect square positions remain ON.

The answer is simply the count of perfect squares less than or equal to n:

⌊
n
	​

⌋
