# LeetCode_Coding-_series
414. Third Maximum Number
Given an integer array nums, return the third distinct maximum number in this array. If the third maximum does not exist, return the maximum number.

Input: nums = [3,2,1]
Output: 1
Explanation:
The first distinct maximum is 3.
The second distinct maximum is 2.
The third distinct maximum is 1.

Input: nums = [1,2]
Output: 2
Explanation:
The first distinct maximum is 2.
The second distinct maximum is 1.
The third distinct maximum does not exist, so the maximum (2) is returned instead.


code : 
class Solution {
    public int thirdMax(int[] nums) {
        long max = Long.MIN_VALUE;
        long secondMax = Long.MIN_VALUE;
        long thirdMax = Long.MIN_VALUE;

        for (int num:nums){
            if (num> max){
                thirdMax = secondMax;
                secondMax = max;
                max = num;
            } else if (num>secondMax && num<max) {
                thirdMax = secondMax;
                secondMax = num;
            } else if (num>thirdMax && num<secondMax) {
                thirdMax = num;
            }
        }
        int result = (thirdMax==Long.MIN_VALUE) ? (int)max : (int)thirdMax;
        return result;
    }
}
