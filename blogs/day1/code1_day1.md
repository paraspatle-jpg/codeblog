**CodeBlog**

Day : 1

Problem solved : 1/4

Problem 1 : # **Puppy and Sum**

[Problem Statement](https://www.codechef.com/problems/PPSUM)

Approach : At First I thought of a very time consuming method to use iteration for finding the sum of natural numbers but then in mid of writing the code I remembered the formulae for finding the sum of N natural numbers.Then I just put the formula and used loop and feed the value of previous sum to the formulae in next loop.

Code:

    #include <bits/stdc++.h>
    using namespace std;
    int main(){
    int t;
    cin>>t;
    while(t--){
      int N , D;
      cin >> D >> N;
      int temp=N;
      int sum  = 0;
      while(D){
        sum=0;
        sum = (temp*(temp+1))/2;
        temp = sum;
        D--;
      }
    cout << sum<<endl;
    }
    }

Time taken : 10 min
