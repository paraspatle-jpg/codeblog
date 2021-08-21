**CodeBlog**

Day : 2

Problem solved : 1/4

Problem 1 : **# Lapindromes**

[Problem Statement](https://www.codechef.com/problems/LAPIN)

Approach : So we have been given a string and we have to check if its lapindrome , I approached the problem using the substring concept , I divided the given string in two halves and stored it in two sub strings using the standard library function substr , then I sorted the sub strings and checked if they are equal ,if they are equal then it is lapindrome , if ther are not equal the its not lapindrome.

Topics: String class , substring,sorting

Code:

    #include <bits/stdc++.h>
    #include<string>
    using namespace std;
    int main() {
    	int t;
    	cin >> t;
    	while(t--){
    	   string lapin;
    	   cin>>lapin;
    	   if(lapin.length()%2==0)
    	   {
    	       string sub1 = lapin.substr(0 , (lapin.length()/2));
    	       string sub2 = lapin.substr((lapin.length()/2));

    	       sort(sub1.begin() , sub1.end());
    	       sort(sub2.begin() , sub2.end());

    	       	   if(sub1 == sub2)
            	   {
            	       cout<<"YES"<<endl;
            	   }
            	   else
            	   {
            	       cout<<"NO"<<endl;
            	   }

    	   }
    	   else
    	   {
    	       string sub1 = lapin.substr(0 , (lapin.length()/2));
    	       string sub2 = lapin.substr((lapin.length()/2)+1);

    	       sort(sub1.begin() , sub1.end());
    	       sort(sub2.begin() , sub2.end());

        	   if(sub1 == sub2)
        	   {
        	       cout<<"YES"<<endl;
        	   }
        	   else
        	   {
        	       cout<<"NO"<<endl;
        	   }
    	   }
    	}
    	return 0;
    	}

Time taken : 20 min
