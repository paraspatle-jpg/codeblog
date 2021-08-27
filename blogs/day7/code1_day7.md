**CodeBlog**

Day : 7

Problem solved : 1/4

Problem : **# Movie Weekend**

[Problem Statement](https://www.codechef.com/problems/MOVIEWKN)

Approach :

Topics: Basic C++

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>         int t;
>         cin>>t;
>         while(t--)
>         {
>             int n;
>             cin>>n;
>             int arr1[n],arr2[n];
>             int index=0;
>             for (int i = 0; i < n; i++)
>                 cin>>arr1[i];
>             for (int i = 0; i < n; i++)
>                 cin>>arr2[i];
>             for (int i = 0; i < n; i++) {
>
>                 if(arr1[index]*arr2[index]== arr1[i]*arr2[i])
>                 {
>                     if(arr2[index]<arr2[i])
>                     {
>                         index = i;
>                     }
>                 }
>                 if(arr1[index]*arr2[index] < arr1[i]*arr2[i]){
>                     index = i;
>                 }
>             }
>
>             cout<<index+1<<endl;
>         }
>     	return 0;
>     }

Time taken : 12 min
