# Regular-Numbers
finds numbers whose only prime divisors are 2, 3, and 5.

Formally, a regular number is an integer of the form $2^i·3^j·5^k$, for nonnegative integers i, j, and k. Such a number is a divisor of $\scriptstyle 60^{\max(\lceil i\,/2\rceil,j,k)}{}$. The regular numbers are also called 5-smooth, indicating that their greatest prime factor is at most 5.

The first few regular numbers are

1, 2, 3, 4, 5, 6, 8, 9, 10, 12, 15, 16, 18, 20, 24, 25, 27, 30, 32, 36, 40, 45, 48, 50, 54, 60, ... 

Although the regular numbers appear dense within the range from 1 to 60, they are quite sparse among the larger integers. A regular number $n = 2^i·3^j·5^k$ is less than or equal to N if and only if the point (i,j,k) belongs to the tetrahedron bounded by the coordinate planes and the plane

$$
(\ln 2)i+(\ln 3)j+(\ln 5)k\le\ln N,
$$

as can be seen by taking logarithms of both sides of the inequality $2^i·3^j·5^k ≤ N$. Therefore, the number of regular numbers that are at most N can be estimated as the volume of this tetrahedron, which is

$$
\frac{\log_2 N\,\log_3 N\,\log_5 N}{6}.
$$

Even more precisely, using big O notation, the number of regular numbers up to N is


$$
\frac{\left(\ln(N\sqrt{30})\right)^3}{6\ln 2 \ln 3 \ln 5}+O(\log N),
$$

and it has been conjectured that the error term of this approximation is actually $$O(\log\log N)$$.

####Example:
Generates the sequence of Regular numbers, in increasing order. In particular:
1. Shows the first twenty Regular numbers.
2. Shows the 1691st Regular number (the last one below 231).
3. Shows the one millionth Regular number
