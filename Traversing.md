- Enumerate function can be used in loop to get the index and the value 
- Range function can be used to traverse the indexes in certain range 
- Len function can be used to get the length of the list 

```python
def twoSum(self, nums: List[int], target: int) -> List[int]: 
    for i,val in enumerate(nums): 
		comp = target-val 
		for j in range(i+1, len(nums)): 
			if i==j: 
				continue 
			if comp == nums[j]: 
				return [i, j] 
```

### Traversing from 0 

```python
for i in range(len(nums))
```