# Sorting

## Selection Sort

- Iterate  i from '0' - (n-1)
- min = i;
- Iterate j from i+1 to n
- if array at index j < array index min
- set min value to j else nothing
- after loop swap array at ith index to array at min index

### **</>**

```cpp
for(int i=0;i<n-1;i++) {
	min = i;
	for(int j=i+1;j<n;j++){
		if(arr[j]<arr[min]){
			min = j;
		}
	}
	swap(arr[i],arr[min]);
}
```

[Tracing](https://www.notion.so/0fe40d5ed404467584c5dbe7b94b81c3)

---

 

## Bubble Sort

- Iterate i from 1 to n
- set flag to 0
- Iterate j from 0 to n-i
- if array at j+1 < array at j
- Swap
- Set Flag to 1
- after loop j if  flag==0 break ( the array is in sorted list )

```cpp
for(int i=1;i<n;i++){
	flag = 0;
	for(int j=0;j<n-i;j++){
		if(arr[j] > arr[j+1] ) {
				Swap (arr[j], arr[j+1])
				flag = 1;
		}
	}
	if(flag ==0 ) {
			break;
	}
}

```

[Tracing](https://www.notion.so/646ff3c56aa04bf78872bdfe57190935)

---

## Insertion Sort

- Iterate i from 1 to n
- initialize temp = array at index i
- Iterate j , j=1 ; j >0 && temp < array [ j-1]  ;  j - -
- array [ j ]  = array [ j - 1 ]
- assign array[ j ] = temp

[ Tracing](https://www.notion.so/e17e4af2149a47f0a5343fe4b46298a9)