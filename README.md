# Practice-3-
Generating All Subarrays
Given an array, arr[], generate all possible subarrays using recursion and return them as a vector of vectors.
The subarrays must be returned in the following order:
      1. Subarrays starting from the first element, followed by subarrays starting from the second element, and so on.
      2. For each starting index, subarrays should be in increasing length.

      <b>
      // User function Template for Java
class Solution {
    public List<List<Integer>> getSubArrays(int[] arr) {
        // code here
        int n = arr.size();
        for (int i = 0 ; i < n ; i++){
            for  ( int j = i ;j < n ; j++){
                for ( int k = i ; k <= j ; k ++){
                    System.out.print(arr.get(k) + " ");
                }  
               System.out.println();
            }
        }
    }
}


Remove Duplicates Sorted Array

<b>
Given a sorted array arr. Return the size of the modified array which contains only distinct elements.
Note:
1. Don't use set or HashMap to solve the problem.
2. You must return the modified array size only where distinct elements are present and modify the original array such that all the distinct elements come at the beginning of the original array

class Solution {
    // Function to remove duplicates from the given array
    public int removeDuplicates(int[] arr) {
        int k = 0; 
        // Code Here
        for ( int i = 0 ; i< arr.length; i ++){
            if ( arr[i]!= arr[k]){
                arr[++k]=arr[i];
            }
        }
        return ++k ;
    }
}

Generating All Subarrays




