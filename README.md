<div align="center">

# ⚡ Daily CP

**One problem a day. Every day. No excuses.**

A running log of my competitive programming practice: solutions, notes, and the mistakes that taught me the most.

![Language](https://img.shields.io/badge/language-C%2B%2B17-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Problems Solved](https://img.shields.io/badge/solved-0-brightgreen?style=for-the-badge)
![Streak](https://img.shields.io/badge/streak-0%20days-orange?style=for-the-badge&logo=fireship&logoColor=white)
![Last Commit](https://img.shields.io/github/last-commit/YOUR_USERNAME/YOUR_REPO?style=for-the-badge&color=blueviolet)

[![Codeforces](https://img.shields.io/badge/Codeforces-YOUR_HANDLE-1F8ACB?style=flat-square&logo=codeforces&logoColor=white)](https://codeforces.com/profile/YOUR_HANDLE)
[![LeetCode](https://img.shields.io/badge/LeetCode-YOUR_HANDLE-FFA116?style=flat-square&logo=leetcode&logoColor=white)](https://leetcode.com/YOUR_HANDLE)
[![CodeChef](https://img.shields.io/badge/CodeChef-YOUR_HANDLE-5B4638?style=flat-square&logo=codechef&logoColor=white)](https://www.codechef.com/users/YOUR_HANDLE)
[![AtCoder](https://img.shields.io/badge/AtCoder-YOUR_HANDLE-222222?style=flat-square&logo=atcoder&logoColor=white)](https://atcoder.jp/users/YOUR_HANDLE)

</div>

---

## 📖 Contents

- [Why this repo exists](#-why-this-repo-exists)
- [Progress](#-progress)
- [Repo structure](#-repo-structure)
- [Topic tracker](#-topic-tracker)
- [Solution template](#-solution-template)
- [Daily log](#-daily-log)
- [Running locally](#-running-locally)

---

## 🎯 Why this repo exists

Consistency beats intensity. Solving one problem a day builds pattern recognition far faster than occasional marathon sessions. Each solution here comes with the approach, complexity, and, when I got it wrong, what I missed.

**Goals**

- Reach **Specialist → Expert** on Codeforces by the end of the year
- Solve **365 problems** with written notes
- Cover every core topic at least 20 problems deep

---

## 📊 Progress

| Platform | Solved | Rating / Rank |
| :-- | :--: | :-- |
| Codeforces | 0 | — |
| LeetCode | 0 | — |
| CodeChef | 0 | — |
| AtCoder | 0 | — |
| **Total** | **0** | |

**Difficulty split**

| Easy | Medium | Hard |
| :--: | :--: | :--: |
| 0 | 0 | 0 |

<div align="center">

![Contribution graph](https://github-readme-streak-stats.herokuapp.com/?user=YOUR_USERNAME&theme=tokyonight&hide_border=true)

</div>

---

## 🗂 Repo structure

```
.
├── codeforces/
│   └── 1850A_to_my_dearest_friend.cpp
├── leetcode/
│   └── 0001_two_sum.cpp
├── codechef/
├── atcoder/
├── templates/
│   ├── base.cpp              # fast IO + macros
│   ├── dsu.cpp
│   ├── segment_tree.cpp
│   └── modint.cpp
├── notes/
│   └── dp_patterns.md
└── README.md
```

**Naming convention:** `<problemID>_<short_snake_case_title>.<ext>`

---

## 🧠 Topic tracker

| Topic | Solved | Confidence |
| :-- | :--: | :-- |
| Arrays & Two Pointers | 0 | ⭐⭐⭐☆☆ |
| Binary Search | 0 | ⭐⭐☆☆☆ |
| Greedy | 0 | ⭐⭐⭐☆☆ |
| Dynamic Programming | 0 | ⭐⭐☆☆☆ |
| Graphs (BFS / DFS) | 0 | ⭐⭐☆☆☆ |
| Shortest Paths | 0 | ⭐☆☆☆☆ |
| Trees & LCA | 0 | ⭐☆☆☆☆ |
| DSU | 0 | ⭐⭐☆☆☆ |
| Number Theory | 0 | ⭐☆☆☆☆ |
| Segment Tree / BIT | 0 | ⭐☆☆☆☆ |
| Strings | 0 | ⭐⭐☆☆☆ |
| Bit Manipulation | 0 | ⭐⭐☆☆☆ |

---

## 🧩 Solution template

Every solution starts with this header so the repo stays searchable:

```cpp
/*
 * Problem : Title (link)
 * Platform: Codeforces | Difficulty: 1200 | Tags: greedy, sortings
 * Date    : YYYY-MM-DD
 *
 * Idea    : One or two lines on the key insight.
 * Time    : O(n log n)
 * Space   : O(n)
 * Mistake : What tripped me up (if anything).
 */
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false);
    cin.tie(nullptr);

    int t; cin >> t;
    while (t--) {
        // solve
    }
    return 0;
}
```

---

## 📅 Daily log

| Date | Problem | Platform | Difficulty | Topic | Solution |
| :-- | :-- | :-- | :--: | :-- | :--: |
| 2026-10-14 | Example Problem | Codeforces | 1200 | Greedy | [📄](codeforces/0000_example.cpp) |

<details>
<summary><b>Older entries</b></summary>

<!-- Move older rows here to keep the main table short -->

</details>

---

## ⚙️ Running locally

```bash
# compile
g++ -std=c++17 -O2 -Wall -o sol codeforces/1850A_to_my_dearest_friend.cpp

# run with sample input
./sol < input.txt
```

---

<div align="center">

If this helps you build your own streak, drop a ⭐

*Keep solving. Keep logging. Keep improving.*

</div>
