# Java Programming Template

A compact Java template for faster implementation during coding contests. Includes common helper classes, algorithms, and input utilities.

---

# Classes

## `IO` — Fast Input Utilities
**Purpose:** Read input with minimal boilerplate.

- `next()` — next space-separated token
- `i()` — integer
- `l()` — long
- `line()` — full line
- `iArr(n)` — integer array of size `n`
- `lArr(n)` — long array of size `n`
- `sArr(n)` — string array of size `n`

---

## `Mod` — Modular Arithmetic
**Purpose:** Arithmetic operations under `1e9+7`.

- `add(a,b)` — compute `(a + b) % MOD`
- `sub(a,b)` — compute `(a - b) % MOD`
- `mul(a,b)` — compute `(a × b) % MOD`
- `inv(a)` — modular inverse
- `div(a,b)` — compute `(a / b) % MOD`

---

## `Mth` — Mathematical Utilities
**Purpose:** Common number theory utilities.

- `gcd(a,b)` — greatest common divisor
- `lcm(a,b)` — least common multiple
- `pow(b,e,m)` — fast modular exponentiation
- `prime(n)` — primality test
- `sieve(n)` — sieve of Eratosthenes

---

## `Arr` — Array Utilities
**Purpose:** Binary search and prefix/suffix preprocessing.

- `lb(arr,x)` — first index where value ≥ `x`
- `ub(arr,x)` — first index where value > `x`
- `pSum(arr)` — prefix sum array
- `sSum(arr)` — suffix sum array
- `pMin(arr)` — prefix minimum array
- `sMin(arr)` — suffix minimum array
- `pMax(arr)` — prefix maximum array
- `sMax(arr)` — suffix maximum array
- `pGcd(arr)` — prefix gcd array
- `sGcd(arr)` — suffix gcd array

---

## `Stk` — Monotonic Stack
**Purpose:** Solve Next Greater Element and similar problems.

- `nge(arr)` — next greater element values
- `ngei(arr)` — next greater element indices

---

## `Grd` — Grid Algorithms
**Purpose:** Grid traversal helpers.

- `ok(r,c,R,C)` — cell in bounds
- `dfs(r,c,grid,vis)` — depth-first search
- `bfs(r,c,grid,vis)` — breadth-first search

---

## `DSU` — Disjoint Set Union
**Purpose:** Track connected components efficiently.

- `find(x)` — find representative
- `union(a,b)` — merge sets
- `same(a,b)` — check connectivity

---

## `ST` — Segment Tree
**Purpose:** Range query + point update structure.

- `upd(idx,val)` — update a value
- `q(l,r)` — query range sum over `[l, r]`

---

## `Bit` — Bit Manipulation
**Purpose:** Common bit operations for integers.

- `get(x,k)` — get the k-th bit of `x`
- `set(x,k)` — set the k-th bit of `x`
- `toggle(x,k)` — toggle the k-th bit of `x`
- `clear(x,k)` — clear the k-th bit of `x`

---

## `Gen` — Test Case Generator
**Purpose:** Create random and edge-case test data.

- `i(min,max)` — random integer
- `l(min,max)` — random long
- `iArr(size,min,max)` — random int array
- `edgeArr(size)` — edge-case array
- `str(len)` — random lowercase string

---

## `DBG` — Debug Utilities
**Purpose:** Print debug information during development.

- `log(name,val)` — log variable value
- `grid(name,grid)` — print 2D grid
- `msg(text)` — print debug message

---

# Debug Mode

```java
public static final boolean DEBUG = true;
```

Set `DEBUG = false` before submitting your solution.

---

# Quick Example

```java
int[] a = IO.iArr(n);
long g = Mth.gcd(a, b);
int pos = Arr.lb(sortedArray, x);

DSU dsu = new DSU(n);
dsu.union(u, v);

ST seg = new ST(values);
long sum = seg.q(l, r);
long ans = Mod.mul(x, y);

int mask = Bit.set(0, 3);
int bit = Bit.get(mask, 3);
```
