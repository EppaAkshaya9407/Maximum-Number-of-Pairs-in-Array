# Maximum-Number-of-Pairs-in-Array
class Solution:
    def numberOfPairs(self, nums: list[int]) -> list[int]:
        if nums is None:
            return None
        r=0
        r1=0
        count=Counter(nums)
        for i,c in count.items():
           r+=c//2
           r1+=c%2
        return [r,r1]
