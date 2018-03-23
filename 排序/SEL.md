# 选择排序

```
for (i = 0; i < 4; i++) { // 4 passes
  cur_min = i;
  for (j = i+1; j < n; j++)
    if (A[j] < A[cur_min])
      cur_min = j;
  swap(A[i], A[cur_min]);
}
```