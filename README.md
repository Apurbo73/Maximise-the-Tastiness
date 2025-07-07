# Maximise-the-Tastiness


---

### ✅ **Problem Recap**:

Chef has 4 ingredients:

* First ingredient can be **A** or **B** → with tastiness values `a` and `b`
* Second ingredient can be **C** or **D** → with tastiness values `c` and `d`

Chef wants to **choose one from A or B**, and **one from C or D**, to make a dish with the **maximum possible tastiness**.

---

### ✅ **Code Explanation**:

```cpp
#include <iostream>
#include <algorithm>
using namespace std;
```

* These lines include necessary libraries.
  `iostream` is for input/output.
  `algorithm` is used for the `max()` function.

---

```cpp
int main() {
    int T;
    cin >> T;
```

* Start of `main()` function.
* Read the number of test cases `T`.

---

```cpp
    while (T--) {
        int a, b, c, d;
        cin >> a >> b >> c >> d;
```

* Loop through all test cases.
* Read the four tastiness values `a`, `b`, `c`, and `d`.

---

```cpp
        int maxTastiness = max(a, b) + max(c, d);
        cout << maxTastiness << endl;
```

* Compute the **maximum tastiness** by:

  * Taking the higher of `a` and `b`
  * Taking the higher of `c` and `d`
  * Adding them together
* Print the result.

---

```cpp
    }

    return 0;
}
```

* End of loop and program.

---

### 🔢 **Example:**

If input is:

```
1
5 7 3 6
```

Then:

* Choose max(5, 7) = 7
* Choose max(3, 6) = 6
* Output: 7 + 6 = **13**

---

