**CodeBlog**

Day : 1

Problem solved : 3/4

Problem 1 : **# Chef and Cook-Off**

[Problem Statement](https://www.codechef.com/submit/CCOOK)

Approach : At first i thought of using a 2d array but later I figured that i dont need it i just need to get the input and check if its one if its one then store it in a array which contains the count of question solved by competitors

Code:

    #include <bits/stdc++.h>
    using namespace std;
    int main() {
    int n;
    cin>>n;
    int input;
    int temp[n]={0};

    int k=0;
    for(int i=0 ; i<n ;i++)
    {
        for (int j =0 ; j<5 ; j++)
        {
            cin >> input;
            if(input==1)
            {
                temp[k]++;
            }
        }
        k++;
    }

    for(int i =0; i<n ; i++)
    {
        if(temp[i]==0)cout<<"Beginner"<<endl;
        if(temp[i]==1)cout<<"Junior Developer"<<endl;
        if(temp[i]==2)cout<<"Middle Developer"<<endl;
        if(temp[i]==3)cout<<"Senior Developer"<<endl;
        if(temp[i]==4)cout<<"Hacker"<<endl;
        if(temp[i]==5)cout<<"Jeff Dean"<<endl;
    }
    return 0;
    }

Time taken : 13 min
