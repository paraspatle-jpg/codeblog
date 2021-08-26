**CodeBlog**

Day : 6

Problem solved : 2/4

Problem : **# Bear and Segment 01**

[Problem Statement](https://www.codechef.com/problems/SEGM01)

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
>     	    string str;
>     	    cin>>str;
>     	    int flag=2;
>     	    for(int i = 0 ; i < str.length() ; i++)
>     	    {
>     	        if(str[i]=='1')
>     	        {
>     	            flag--;
>     	            if(flag ==0)break;
>     	            while(str[i] != '0')
>     	            {
>
>     	                i++;
>     	                if(i==str.length())break;
>     	            }
>     	        }
>
>     	    }
>     	    if(flag==1)cout<<"YES"<<endl;
>     	    else cout<<"NO"<<endl;
>     	}
>     	return 0;
>     }

Time taken : 15 min
