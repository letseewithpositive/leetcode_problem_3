# leetcode_problem_3
solution of leetcode problem 89
class Solution {
public:
    vector<int> grayCode(int n) {
        vector<int> ans;
        for(int i=0;i<pow(2,n);i++){
            ans.push_back((i>>1)^i);
        }
        return ans;
    }
};
