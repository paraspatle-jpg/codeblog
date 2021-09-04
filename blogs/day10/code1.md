**CodeBlog**

Day : 10

Problem solved : 1/4

Problem : **# Chef and Eid**

[Problem Statement](https://www.codechef.com/problems/EID)

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
>     	while(t--)
>     	{
>     	    int n;
>     	    cin>>n;
>     	    int arr[n];
>     	    for (int i = 0; i < n; i++) {
>     	        cin>>arr[i];
>     	    }
>     	    sort(arr,arr+n);
>     	    int diff=arr[1]-arr[0];
>     	    for (int i = 1; i < n; i++) {
>     	        if(arr[i]-arr[i-1] < diff)
>     	        {
>     	            diff = arr[i] - arr[i-1];
>     	        }
>     	    }
>     	    cout<<abs(diff)<<endl;
>     	}
>     	return 0;
>     }
>
> Time Taken : 8min
