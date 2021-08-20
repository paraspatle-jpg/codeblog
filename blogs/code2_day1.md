**CodeBlog**

Day : 1

Problem solved : 2/4

Problem 2 : **# Packaging Cupcakes**

[Problem Statement](https://www.codechef.com/problems/MUFFINS3)

Approach : It is a very simple problem on usage of if else ladder , we just have to form packages, such that only one biggest pakage is formed and if cupcakes are less that or equal to 2 then there wil;l be cupcakes left irrespective of the size of package
Code:

    #include<bits/stdc++.h>
    using namespace std;
    int main(){
    int t;
    cin >> t;
    while(t--)
    {
        int cupcakes;
        cin >> cupcakes;
        if (cupcakes <= 2)
        {
            cout<< cupcakes<<endl;
        }
        else if(cupcakes >2 && cupcakes % 2 ==0)
        {
            cout << (cupcakes/2)+1<< endl;
        }
        else if(cupcakes >2 && cupcakes % 2 !=0)
        {
            cout << (cupcakes+1)/2<<endl;
        }
    }
    }

Time taken : 8 min
