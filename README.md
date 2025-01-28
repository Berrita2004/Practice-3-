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
