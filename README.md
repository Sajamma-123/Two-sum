class Solution:
    def twoSum(self, arr , target):
        ans=[0]*2
        d={}
        for i in range(len(arr)):
            diff=target-arr[i]
            if(diff in d):
                ans[0]=d[diff]
                ans[1]=i
            d[arr[i]]=i
        return ans
