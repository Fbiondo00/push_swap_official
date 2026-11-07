# push_swap

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white) ![Algorithms](https://img.shields.io/badge/Algorithms-7209B7?style=flat-square) ![42 Roma Luiss](https://img.shields.io/badge/42_Roma_Luiss-000000?style=flat-square&logo=42&logoColor=white)

Sort a list of integers using two stacks, `a` and `b`, and a limited set of operations (`sa` `sb` `pa` `pb` `ra` `rb` `rra` `rrb` …), with as few moves as possible.

## Strategy

- **2–5 numbers**: hand-written routines that find the optimal moves
- **Larger inputs**: **binary radix sort**, using the two stacks as buckets

## Build & run

```bash
make
./push_swap 3 2 5 1 4
ARG="$(seq 1 100 | sort -R | tr '\n' ' ')"; ./push_swap $ARG | wc -l
```

---

<sub>Part of my 42 Roma Luiss curriculum · [more projects](https://github.com/Fbiondo00) · MIT License</sub>
