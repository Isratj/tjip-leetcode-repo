Add your week-01's solution to this directory.
Create a seperate file for each of your solution. Name the file according to the problem name.

PYTHON:
def twoSum(self, nums: List[int], target: int) -> List[int]:
        hash_map = {}
        for i in range(len(nums)):
            if nums[i] in hash_map:
                return [i, hash_map[nums[i]]]
            else:
                hash_map[target - nums[i]] = i
 C++:
 
/* C++ Program to find sum of elements 
in a given array */
#include <bits/stdc++.h>
using namespace std;
  
// function to return sum of elements 
// in an array of size n 
int sum(int arr[], int n) 
{ 
    int sum = 0; // initialize sum 
  
    // Iterate through all elements 
    // and add them to sum 
    for (int i = 0; i < n; i++) 
    sum += arr[i]; 
  
    return sum; 
} 
  
// Driver code
int main() 
{ 
    int arr[] = {12, 3, 4, 15}; 
    int n = sizeof(arr) / sizeof(arr[0]); 
    cout << "Sum of given array is " << sum(arr, n); 
    return 0; 
} 
