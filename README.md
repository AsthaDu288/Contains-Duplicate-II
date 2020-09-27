# Contains-Duplicate-II
We need find out whether there are two distinct indices i and j in the array such that nums[i] = nums[j] and the absolute difference between i and j is at most k.
class Solution {
    public boolean containsNearbyDuplicate(int[] nums, int k) {
        for(int i=0;i<nums.length;i++){
            for(int j=i+1;j<nums.length;j++){
                if(nums[i] == nums[j]){
                    if(Math.abs(i-j) <= k){
                        return true;
                    }
                   
                }
            }
        }
        return false;
    }
}
