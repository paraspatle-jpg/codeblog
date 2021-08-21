**CodeBlog**

Day : 2

Problem solved : 2/4

Problem 2 : **# Chef and Dolls**

[Problem Statement](https://www.codechef.com/problems/MISSP)

Approach : We have been given an odd numbers of dolls which are in pair we have to find the doll whose pair was stolen,for this we will store the dolls in array and then sort the array and see if the a number has its adjacent number equal or not, if it is not equal then return that doll as output.

Topics: Sorting

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>     	int t ;
>     	cin>>t;
>     	while (t--){
>     	    int n;
>     	    cin>> n;
>     	    int arr[n];
>     	    int flag =1;
>     	    for(int i =0 ; i<n ; i++)
>     	    {
>     	        cin>>arr[i];
>     	    }
>     	    sort(arr , arr+n);
>     	    for(int i =1 ; i<n-1 ; i=i+2){
>     	        if(arr[i]!=arr[i-1])
>     	        {
>     	            flag =0;
>     	            cout<<arr[i-1]<<endl;
>     	            break;
>     	        }
>     	    }
>     	    if(flag)
>     	    {
>     	       cout<<arr[n-1]<<endl;
>     	    }
>     	}
>     	return 0;
>     }

Time taken : 10 min
