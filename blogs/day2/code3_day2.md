**CodeBlog**

Day : 2

Problem solved : 3/4

Problem 3 : **# Chocolate Monger**

[Problem Statement](https://www.codechef.com/problems/CM164364)

Approach :

Topics: Vector,sorting

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
>     	    int c,x;
>     	    cin>>c>>x;
>     	    int arr[c];
>     	    for(int i =0 ; i <c ; i++)
>     	    {
>     	        cin>>arr[i];
>     	    }
>     	    sort(arr,arr+c);
>     	    vector<int>temp;
>     	    temp.push_back(arr[0]);
>     	    for(int i =1;i<c;i++)
>     	    {
>     	        if(temp.back()!=arr[i]){
>     	            temp.push_back(arr[i]);
>     	        }
>     	    }
>     	    if(c - temp.size() >= x)
>     	    {
>     	        cout<<temp.size()<<endl;
>     	    }
>     	    else
>     	    {
>     	        cout<<c-x<<endl;
>     	    }
>     	}
>     	return 0;
>     }

Time taken : 20 min
