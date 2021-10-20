# 20211020-

#LeetCode 961. N-Repeated Element in Size 2N Array
class Solution:
    def repeatedNTimes(self, nums: List[int]) -> int:
        n = len(nums)//2
        for i in range(n+1):
            count = nums.count(nums[i])
            if count == n:
                return nums[i]
