# Microsoft Excel - Module 3  
## AND and OR Functions



## 📘 Introduction

At this stage of the course, you should be familiar with logical functions in Microsoft Excel like the `IF` and `IFS` functions. Another method of enhancing the performance of these functions is using the `AND` and `OR` functions.

In this reading, I learn how to use these functions to test multiple conditions simultaneously.



## 🔍 The AND Function

The `AND` function allows Excel to perform **multiple logical tests at once**. It can take up to 30 arguments (conditions), and:

- Returns `TRUE` only if **all conditions are TRUE**
- Returns `FALSE` if **any one condition is FALSE**

### ✅ Syntax

```excel
=AND(condition1, condition2, ..., condition30)
```

### 🧪 Example 1

```excel
=AND(A2<200, B2<200, C2<200)
```

- A2 = 50, B2 = 100, C2 = 150 → ✅ `TRUE`
- All values are less than 200
  ![image](https://github.com/user-attachments/assets/885ee525-bd74-455a-b081-cb8834a7bfe8)


### ❌ Example 2

```excel
=AND(A2<200, B2<200, C2<200)
```

- C2 = 250 → ❌ `FALSE`
- One test failed
  ![image](https://github.com/user-attachments/assets/a46f376d-033a-44b0-85c7-bd336354c7f8)




## 🔍 The OR Function

The `OR` function also checks multiple conditions. It returns:

- `TRUE` if **at least one** condition is `TRUE`
- `FALSE` only if **all** conditions are `FALSE`

### ✅ Syntax

```excel
=OR(condition1, condition2, ..., condition30)
```

### 🧪 Example 1

```excel
=OR(A2<200, B2<200, C2<200)
```

- A2 = 100, B2 = 300, C2 = 400 → ✅ `TRUE`
- One test passed
![image](https://github.com/user-attachments/assets/5f66bf67-578a-4e6a-a520-07b97c96b9aa)

### ❌ Example 2

```excel
=OR(A2<200, B2<200, C2<200)
```

- A2 = 250, B2 = 300, C2 = 400 → ❌ `FALSE`
- No test passed

![image](https://github.com/user-attachments/assets/aaf97b4c-d169-4056-acfd-226bd4c6c3a7)


## 🔄 Using AND with IF

The `AND` function is often used **within** an `IF` function to check multiple conditions and return custom messages.

### ✅ Syntax

```excel
=IF(AND(condition1, condition2), "True Result", "False Result")
```

### 🧪 Example

```excel
=IF(AND(A2>200, B2>200), "On Target", "Target Not Met")
```

- A2 = 300, B2 = 400 → ✅ "On Target"
  ![image](https://github.com/user-attachments/assets/12ba75ad-9c2f-4bb3-9fc6-31e5683917d7)

- If either ≤ 200 → ❌ "Target Not Met"

![image](https://github.com/user-attachments/assets/5dc9ab47-6a1d-48cf-82ab-52ad94eba77d)


## 🏁 Conclusion

In this module, I learned how:

- The `AND` function requires **all conditions** to be true  
- The `OR` function requires **at least one condition** to be true  
- Both can be combined with `IF` to build **dynamic logic**

These functions enhance the decision-making power of My Excel formulas and help create more intelligent spreadsheets.

---

