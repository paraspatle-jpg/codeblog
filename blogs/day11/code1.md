**CodeBlog**

Day : 11

Problem solved : 1/4

Problem : **# Travel Pass**

[Problem Statement](https://www.codechef.com/SEPT21C/problems/TRAVELPS)

Approach :

Topics: Basic C++

> Code:
>
>     #include <bits/stdc++.h>
>
>     using  namespace std;
>     int main()
>     {
>     int t;
>     cin >> t;
>     while (t--)
>     {
>     int n, a, b;
>     string str;
>     cin >> n >> a >> b;
>     cin >> str;
>     int time = 0;
>     for (int i = 0; i < n; i++)
>     {
>     if (str[i] == '0')
>     time = time + a;
>     else
>     time = time + b;
>     }
>     cout << time << endl;
>     }
>     return  0;
>     }

Time Taken : 8min
