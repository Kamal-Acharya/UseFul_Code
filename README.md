# HeaderFiles
- #include <iostream>
- using namespace std;
- #define fo(i,n) for(int i=0; i<n; i++)
- #define FO(i,a,n) for(int i=a; i<n; i++)
- #define deb(x) cout << #x << " " << x << "\n";
- #define pb push_back
- #define mp make_pair
- #define F first
- #define S second
- #define el "\n"
- #define pel cout << "\n";
- #define accuracy setprecision(20)
- #define vi vector<int>
- #define vll vector<ll>
- #define vpii vector<pair<int, int>>
- #define vpll vector<pair<ll, ll>>
- #define mii map<int, int>
- #define all(x) x.begin(), x.end()
- typedef long long int ll;
- typedef long double ld;
- const ll mod = 1e9+7;
- const ll mod1 = 998244353;
- const long double Pi = acos(-1);
- const long double euler= 2.7182818284590452353602;
  ---
  # To check Prime or NOT
  ```c++
   bool isPrime(ll n)
   if (n <= 1)  return false; 
   if (n <= 3)  return true; 
   if (n%2 == 0 || n%3 == 0) return false; 
   for (ll i=5; i*i<=n; i=i+6) 
   if (n%i == 0 || n%(i+2) == 0) 
   return false; 
   return true; 

  ```
 # IsPerfect
 ```c++
 bool isPerfect(ll n)
 {
 ll x = sqrt(n);
 if(x*x==n) return true;
 else return false;
 }
 ```
# Ceil of Number
```c++
ll ceilInt(ll a, ll b)
{
if(a%b==0) return a/b;
else return a/b +1;
}
```                       
