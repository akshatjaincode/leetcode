# leetcode
//leetcode 1574 c++ code

class Solution {
public:
    int findLengthOfShortestSubarray(vector<int>& arr) {
        int n=arr.size();
        int c=0;
        int left = 0;
        int right = n-1;
        while(left<=right){
            if(left==right){
                left=left-1;
            }
            if(arr[left]>arr[right]){
                c++;
            }
            left++;
            right--;
        }
        if(c==0){
            return c;
        }

          else  
    return c+1;
        }
    
};
