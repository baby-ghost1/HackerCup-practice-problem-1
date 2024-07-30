# HackerCup-practice-problem-1
C++ solution of meta hackercup practice problem 1

#include <bits/stdc++.h>
using namespace std;
int main() {
    int t; cin >> t;
    for(int i = 1; i <= t; i++) {
        int s, d, k;
        cin >> s >> d >> k;

        int buns = 2*(s+d);
        int patties = s + 2*d;
        int cheese = s + 2*d;

        if( buns >= k+1 && k <= min(patties, cheese)) cout <<"Case #"<<i<<": "<<"YES\n";
        else cout<<"Case #"<<i<<": "<<"NO\n";
    }
}
