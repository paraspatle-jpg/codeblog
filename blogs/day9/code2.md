**CodeBlog**

Day : 9

Problem solved : 2/4

Problem : **# CONSISTENCY PART 1 / facebook Hackercup**

[Problem Statement](https://www.facebook.com/codingcompetitions/hacker-cup/2021/qualification-round/problems/A1)

Approach :

Topics: Basic C++

> Code:
>
>     #include <bits/stdc++.h>
>
>     using  namespace std;
>
>
>
>     char MaxOccuringChar(string str)
>
>     {
>
>     int count[95] = {0};
>
>
>
>     int len = str.length();
>
>     int max = 0;
>
>     char result;
>
>
>
>     for (int i = 0; i < len; i++)
>
>     {
>
>     count[str[i]]++;
>
>     if (max < count[str[i]])
>
>     {
>
>     max = count[str[i]];
>
>     result = str[i];
>
>     }
>
>     }
>
>     return result;
>
>     }
>
>
>
>     int main()
>
>     {
>
>     int t, p = 0;
>
>     cin >> t;
>
>     while (t--)
>
>     {
>
>     p++;
>
>     string s;
>
>     cin >> s;
>
>     string vowel, consonant;
>
>     for (int i = 0; i < s.length(); i++)
>
>     {
>
>     if (s[i] == 'A' || s[i] == 'E' || s[i] == 'I' || s[i] == 'O' || s[i] == 'U')
>
>     {
>
>     vowel.append(s, i, 1);
>
>     }
>
>     else
>
>     {
>
>     consonant.append(s, i, 1);
>
>     }
>
>     }
>
>     int maxv, maxc;
>
>     char max_vowel = MaxOccuringChar(vowel);
>
>     char max_consonant = MaxOccuringChar(consonant);
>
>
>
>     int timev = 0, timec = 0;
>
>     for (int i = 0; i < s.length(); i++)
>
>     {
>
>     if (s[i] == 'A' || s[i] == 'E' || s[i] == 'I' || s[i] == 'O' || s[i] == 'U')
>
>     {
>
>     timec++;
>
>     if (s[i] != max_vowel)
>
>     {
>
>     timev = timev + 2;
>
>     }
>
>     }
>
>     else
>
>     {
>
>     timev++;
>
>     if (s[i] != max_consonant)
>
>     {
>
>     timec = timec + 2;
>
>     }
>
>     }
>
>     }
>
>
>
>     if (timec > timev)
>
>     cout << "Case #" << p << ": " << timev << endl;
>
>     else
>
>     cout << "Case #" << p << ": " << timec << endl;
>
>     }
>
>     return  0;
>
>     }

Time taken : 60 min
