**CodeBlog**

Day : 8

Problem solved : 2/4

Problem : **# Total Expenses**

[Problem Statement](https://www.codechef.com/problems/FLOW009)

Approach :

Topics: Basic C++

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>      	 int t;
>          cin>>t;
>          while(t--)
>          {
>     	    double quantity ,price;
>     	    cin>>quantity>>price;
>     	    double result;
>     	    if(quantity > 1000)
>     	    {
>     	        result = quantity*price*0.9;
>     	    }
>     	    else{
>     	        result = quantity*price;
>     	    }
>     	     cout<<fixed<<setprecision(6)<<result<<endl;
>     }
>     return 0;
>     }

Time taken : 5 min
