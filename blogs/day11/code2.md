**CodeBlog**

Day : 11

Problem solved : 2/4

Problem : **# Travel Pass**

[Problem Statement](https://www.codechef.com/SEPT21C/problems/SHUFFLIN)

Approach :

Topics: Basic C++

> Code:
> #include <bits/stdc++.h>
> using namespace std;
> int main()
> {
> int t;
> cin >> t;
> while (t--)
> {
> int n;
> cin >> n;
> int arr[n];
> int even_numbers = 0, odd_numbers = 1;
> int input, sum = 0;
> for (int i = 0; i < n; i++)
> {
> cin >> input;
> if (input != 0)
> {
> if (input % 2 == 0 && even_numbers < n)
> {
> sum++;
> even_numbers = even_numbers + 2;
> }
> else if (input % 2 != 0 && odd_numbers < n)
> {
> sum++;
> odd_numbers = odd_numbers + 2;
> }
> }
> }
> cout << sum << endl;
> }
> return 0;
> }

Time Taken : 8min
