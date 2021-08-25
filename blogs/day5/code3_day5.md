**CodeBlog**

Day : 5

Problem solved : 3/4

Problem : **# Snake Procession**

[Problem Statement](https://www.codechef.com/problems/SNAKPROC)

Approach :

Topics: Basic C++ , Aptitude

> Code:
>
>     #include <bits/stdc++.h>
>
>     using namespace std;
>
>
>
>     int main() {
>
>     int t;
>
>     cin>>t;
>
>     while(t--)
>
>     {
>
>     int l;
>
>     cin>>l;
>
>     string ht;
>
>     cin>>ht;
>
>     int flag = 0 ;
>
>     for (int i = 0; i < l; i++) {
>
>     if(ht[i]=='T')
>
>     {
>
>     flag++;
>
>     break;
>
>     }
>
>     if(ht[i]=='H'){
>
>     while(ht[i]!= 'T')
>
>     {
>
>     i++;
>
>     if(ht[i]== 'H')
>
>     {
>
>     flag++;
>
>     break;
>
>     }
>
>     if(i>l)
>
>     {
>
>     flag++;
>
>     break;
>
>     }
>
>     }
>
>     }
>
>     if(flag) break;
>
>     }
>
>     if(flag)cout<<"Invalid"<<endl;
>
>     else cout<<"Valid"<<endl;
>
>     }
>
>     return 0;
>
>     }

Time taken : 15 min
