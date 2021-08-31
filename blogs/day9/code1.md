**CodeBlog**

Day : 9

Problem solved : 1/4

Problem : **# Closing the Tweets**

[Problem Statement](https://www.codechef.com/problems/TWTCLOSE)

Approach :

Topics: Basic C++

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>     	int n , k;
>     	cin>>n>>k;
>     	int arr[n]={0};
>     	int num,count;
>     	for (int i = 0; i < k; i++) {
>     	    string str;
>     	    cin>>str;
>     	    count =0;
>     	    if(str == "CLICK")
>     	    {
>             cin>>num;
>             arr[num-1]++;
>     	    for(int j = 0 ; j < n ; j++)
>     	    {
>     	        if(arr[j]%2 != 0)
>     	        {
>     	            count++;
>     	        }
>     	    }
>
>     	    cout<<count<<endl;
>     	    }
>
>     	    else{
>     	     for(int j = 0 ; j < n ; j++)
>     	    {
>     	        arr[j]=0;
>     	    }
>     	        cout<<"0"<<endl;
>     	    }
>
>     	}
>     	return 0;
>     }

Time taken : 8 min
