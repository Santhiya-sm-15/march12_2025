# march12_2025
The problem that i solved today in leetcode

1.Given an array nums sorted in non-decreasing order, return the maximum between the number of positive integers and the number of negative integers.

In other words, if the number of positive integers in nums is pos and the number of negative integers is neg, then return the maximum of pos and neg.
Note that 0 is neither positive nor negative.

Code:
class Solution {
    public int maximumCount(int[] nums) {
        int n=nums.length;
        int pos=0,neg=0;
        for(int x:nums)
        {
            if(x>0)
                pos++;
            else if(x<0)
                neg++;
        }
        return Math.max(pos,neg);
    }
}
