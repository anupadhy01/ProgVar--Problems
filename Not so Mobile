#include <iostream>
#include <sstream>
#include <cstdio> 
#include <cmath> 
#include <cstring> 
#include <cctype> 
#include <string> 
#include <vector> 
#include <numeric>
#include <list> 
#include <set> 
#include <map> 
#include <queue> 
#include <stack> 
#include <algorithm> 
#include <functional>
#include <iomanip>
#include <unordered_map>
#include <climits>
#include <bitset>

#include<ext/pb_ds/assoc_container.hpp>
#include<ext/pb_ds/tree_policy.hpp>

using namespace std;
using namespace __gnu_pbds;

typedef tree<int, null_type, less<int>, rb_tree_tag, tree_order_statistics_node_update> PBDS;
typedef tree<pair<int, int>, null_type, less<pair<int, int> >, rb_tree_tag, tree_order_statistics_node_update> PBDS_pair;

#define shift cout<<endl
#define DEBUG(x) cout << '>' << #x << ':' << x << endl; 
#define REP(i,n) for(int i=0;i<(n);i++) 
#define FOR(i,a,b) for(int i=(a);i<=(b);i++) 
#define FORD(i,a,b) for(int i=(a);i>=(b);i--)
#define ps(x, y) fixed<<setprecision(y)<<x  
inline bool EQ(double a, double b) { return fabs(a-b) < 1e-9; } 
 
const int INF = 1<<29; 
typedef long long ll; 
typedef long double lld;
 
inline int two(int n) { return 1 << n; } 
inline int test(int n, int b) { return (n>>b)&1; } 
inline void set_bit(int & n, int b) { n |= two(b); } 
inline void unset_bit(int & n, int b) { n &= ~two(b); } 
inline int last_bit(int n) { return n & (-n); } 
inline int ones(int n) { int res = 0; while(n && ++res) n-=n&(-n); return res; } 
 
template<class T> void chmax(T & a, const T & b) { a = max(a, b); } 
template<class T> void chmin(T & a, const T & b) { a = min(a, b); } 

const long long MOD=1000000007;

void c_p_c()
{
    ios_base::sync_with_stdio(false); cin.tie(NULL); cout.tie(NULL);
    #ifndef ONLINE_JUDGE
        freopen("input.txt", "r", stdin);
        freopen("output.txt", "w", stdout);
    #endif
}

// ############################################

pair<bool, ll> recFx()
{
    ll lw, la, rw, ra;
    cin>>lw>>la>>rw>>ra;
    if(lw==0) { pair<bool, ll> p=recFx(); if(p.first==false) return {false, INF};  lw+=p.second; }
    if(rw==0) { pair<bool, ll> p=recFx(); if(p.first==false) return {false, INF}; rw+=p.second; }
    bool curr=(lw*la==rw*ra);
    if(curr==false) return {false, INF};
    return {true, lw+rw};
}

int32_t main()
{
    c_p_c();
    ll t; cin>>t;
    while(t--)
    {
        if(recFx().first) cout<<"YES\n";
        else cout<<"NO\n";
    }
    return 0;
}
