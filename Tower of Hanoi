#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;

void towerOfHanoi(int n, char src, char dest, char helper)
{
    if(n==1) { cout<<"Move from "<<src<<" to "<<dest<<".\n"; return; }
    towerOfHanoi(n-1, src, helper, dest);
    cout<<"Move from "<<src<<" to "<<dest<<".\n";
    towerOfHanoi(n-1, helper, dest, src);
}

int main() {
    int t; cin>>t;
    while(t--)
    {
        int n; cin>>n;
        char src, dest; cin>>src>>dest;
        char helper='A'+'B'+'C'-src-dest;
        towerOfHanoi(n, src, dest, helper);
        cout<<"Done!\n";
    }
    return 0;
}


