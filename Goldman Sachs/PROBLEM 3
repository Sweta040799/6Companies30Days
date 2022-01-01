# [Link to soltuion](https://practice.geeksforgeeks.org/viewSol.php?subId=dd63e1f1d36caf03251a895a21eaf04c&pid=703804&user=sweta040799)

Code : 
class Solution{
  public:
    int countSubArrayProductLessThanK(const vector<int>& a, int n, long long k) {
        int i = 0,ans = 0;
        long long product = 1;
        
        for(int j=0;j<n;j++){
            product *= a[j];
            
            while(i <= j && product >= k){
                product /= a[i];
                i++;
            }
            
            ans += j-i+1;
        }
        
       return ans;
    }
};
