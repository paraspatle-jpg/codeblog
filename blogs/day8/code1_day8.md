**CodeBlog**

Day : 8

Problem solved : 1/4

Problem : **# Minimum Maximum**

[Problem Statement](https://www.codechef.com/problems/MNMX)

Approach :

Topics: Basic C++

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>     	int t;
>     	cin>>t;
>     	while(t--){
>     	    int n;
>     	    cin>>n;
>     	    long long int min= 100000 , input;
>     	    for (int i = 0; i < n; i++) {
>     	        cin>>input;
>     	        if(input < min){
>     	            min = input;
>     	        }
>     	    }
>     	    cout<<min*(n-1)<<endl;
>     	}
>     	return 0;
>     }

Time taken : 5 min
