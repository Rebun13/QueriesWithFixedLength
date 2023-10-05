# QueriesWithFixedLength

## Description

Consider an _n_-integer sequence, $A = {a_0, a_1, ..., a_{n-1}}$. We perform a query on _A_ by using an integer, _d_, to calculate the result of the following expression:

$$ min_{0≤i≤n-d}(max\ a_j)_{i≤j<i+d} $$

In other words, if we let $m_i = max(a_i, a_{i+1}, a_{i+2}, ..., a_{i+d-1})$, then you need to calculate
$min(m_0, m_1, ..., m_n-d)$.

Given _arr_ and _q_ queries, return a list of answers to each query.

## Returns

- int[q]: the answers to each query

## Input

- The first line consists of two space-separated integers, _n_ and _q_.
- The second line consists of _n_ space-separated integers, the elements of _arr_.
- Each of the _q_ subsequent lines contains a single integer denoting the value of _d_ for that query.
