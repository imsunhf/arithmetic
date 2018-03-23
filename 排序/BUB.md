# 冒泡排序

```
for (j = 0; j < 8; j++) // 8 passes
  for (i = 0; i < n-j-1; i++)
    if (A[i] > A[i+1])
      swap(A[i], A[i+1])
// 2
j = 0;
do {
  swapped = false; j++;
  for (i = 0; i < n-j; i++) // each completion of this for-loop is counted as one pass
    if (A[i] > A[i+1]) { // each execution of this if-statement is counted as one comparison
      swap(A[i], A[i+1]);
      swapped = true;
    }
} while (swapped);
```