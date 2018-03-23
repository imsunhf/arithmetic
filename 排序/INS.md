# 插入排序

```
for (i = 1; i < n; i++) {
  e = A[i]; j = i;
  while (j > 0) {
    if (A[j-1] > e) // each execution of this if-statement is counted as one comparison
      A[j] = A[j-1];
    else
      break;
    j--;
  }
  A[j] = e;
}
```