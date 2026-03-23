# Background
A **Monotonic Stack** is a data structure where elements are always kept in a specific sorted order, either consistently increasing or decreasing
	Consistently increasing or decreasing
# Two Pointers
Iterating two monotonic pointers across an array to search for a pair of indices satisfying some condition in linear time

Very useful for linear data structures like lists, strings, and occasionally linked lists

Using two indices(pointers) in order to avoid nested loops and repetitive scanning

Two Techniques:
	**Same Direction**:
		Single pass over data, but need to track a range, not just one element at a time
		*Example:* Fast-slow pointer
	**Opposite Direction**:
		Used when the array is sorted
		Having one pointer at the first index and having a second pointer at the last index, then checking a condition, then deciding which pointer to move
## Code
Python
```
def two_sum(arr, target):
    n = len(arr)
    for i in range(n):
        for j in range(i + 1, n):
            if arr[i] + arr[j] == target:
                return True
    return False
```

C++
```
#include <bits/stdc++.h>
using namespace std;

int main() {
	ios::sync_with_stdio(false);
	cin.tie(nullptr);

	int N, T;
	cin >> N >> T;
	vector<int> A(N);
	for (int &a : A) cin >> a;

	int r = -1, sum = 0, ans = 0;
	// sum stores sum of A[l ... r inclusive]
	for (int l = 0; l < N; sum -= A[l++]) {
		while (r + 1 < N && sum + A[r + 1] <= T) sum += A[++r];
		ans = max(ans, r - l + 1);
	}
	cout << ans << "\n";
}
```
# Sliding Window
Helpful for problems that ask for continuous segments like substrings or sublists

Similar to Two Pointer Problem, but tighter focus

Two patterns:
	**Fixed window**:
		Used when the problem gives a specific window size or window size is static
		Adding one to the right and deleting one to the left
	**Dynamic Window**:
		Used when the problem does not give a specific window size or the window size is dynamic
		Adding one to the right until the condition is no longer fulfilled, so remove one from the left
## Code
C++
```
#include <vector>
#include <algorithm>
#include <unordered_map> // Or other data structures as needed

using namespace std;

// The general logic involves expanding the right pointer and contracting the left pointer when a condition is met.
int slidingWindowTemplate(vector<int>& nums) {
    int left = 0;
    int right = 0;
    // Use an appropriate data structure (e.g., hash map, set, or simple variables) 
    // to track the state of the current window.
    // Example: unordered_map<int, int> window_state;
    
    int result = 0; // The answer to the problem (max length, min value, etc.)

    while (right < nums.size()) {
        // 1. Expand the window by moving the right pointer
        int element_right = nums[right];
        // CODE: Update window_state to include element_right
        
        right++;

        // 2. Shrink the window if it violates the problem's condition(s)
        while (/* window violates condition */) {
            int element_left = nums[left];
            // CODE: Update window_state to remove/exclude element_left
            
            left++;
        }

        // 3. Update the result (e.g., max/min length, count) after each valid window adjustment
        // result = max(result, right - left); // Example for max length
    }
    
    return result;
}
```
Python
Fixed
```
def fixed_length_sliding_window(nums, k):
    left = 0
    window_state = 0
    result = float('-inf')
    for right in range(len(nums)):
        window_state += nums[right]
        if right - left + 1 == k:
            result = max(result, window_state)
            window_state -= nums[left] 
            left += 1        
    return result
```
Dynamic
```
def dynamic_length_sliding_window(nums):
    left = 0
    window_state = {}
    result = 0

    for right in range(len(nums)):
        window_state[char] = window_state.get(char, 0) + 1
        while window_needs_shrinking(window_state, condition_params): 
            left_char = nums[left]
            window_state[left_char] -= 1
            if window_state[left_char] == 0:
                del window_state[left_char]
            left += 1
        result = max(result, right - left + 1)
    return result
```
# Binary Search
Cutting a sorted linear data structure by cutting the structure in half over and over again
Monotonic vs Non-monotonic

Code:
Python:
```
def binary_search_exact(nums: list[int], target: int) -> int:
    left, right = 0, len(nums) - 1

    while left <= right:
        mid = left + (right - left) // 2 

        if nums[mid] == target:
            return mid
        elif nums[mid] < target:
            left = mid + 1 
        else:
            right = mid - 1

```
C++:
```
#include <iostream>
#include <vector>

// Generic template for binary search
template <typename T>
int binarySearch(const std::vector<T>& arr, const T& target) {
    int left = 0;
    int right = arr.size() - 1;

    while (left <= right) {
        // Prevent potential overflow by using 'left + (right - left) / 2'
        int mid = left + (right - left) / 2;

        if (arr[mid] == target) {
            return mid; // Target found, return index
        } else if (arr[mid] < target) {
            left = mid + 1; // Discard the left half
        } else {
            right = mid - 1; // Discard the right half
        }
    }

    return -1; // Target not found, return -1
}

int main() {
    std::vector<double> data = {1.5, 2.7, 3.1, 4.9, 5.0};
    double target_val = 3.1;

    int index = binarySearch(data, target_val);

    if (index != -1) {
        std::cout << "Element " << target_val << " found at index: " << index << std::endl;
    } else {
        std::cout << "Element " << target_val << " not found." << std::endl;
    }

    return 0;
}

```
# Breadth-First Search(BFS)
One of the most common ways to traverse non-linear structures like graphs and trees

Start at the source node or root, then visit all of the neighbors of the node, but moving down a level

First in first out, using a queue

BFS on a tree is easy as the structure of a tree makes it easy for avoiding repetition

# Depth-First Search(DFS)
Fully explore one branch before moving onto the next

# Resources:
https://www.youtube.com/watch?v=Z_c4byLrNBU


