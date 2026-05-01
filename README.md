# Sort-an-array-2
class Solution {
public:
    vector<int> sortArray(vector<int>& nums) {
        int n=nums.size();
        for(int i=0;i<n-1;i++){
            int min=i;
            for(int j=i;j<n;j++){
                if(nums[j]<nums[min]){
                    min=j;
                }
            }
                    swap(nums[min],nums[i]);
                
        }
        return nums;
       
    }
};
