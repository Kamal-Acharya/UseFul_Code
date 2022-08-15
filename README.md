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
# Binary Search
```c++
int binarySearch(ll arr[], int l, int r, int x) 
{ 
while (l <= r) { 
int m = l + (r - l) / 2; 
if (arr[m] == x&&m!=0) 
return m; 
if (arr[m] < x) 
l = m + 1; 
else
r = m - 1; 
} 
return 0; 
} 
``` 
# Gcd and Lcm 
```c++
ll gcd(long long int a, long long int b)
{
if (b == 0)
return a;
return gcd(b, a % b);
}
ll lcm(ll a, ll b)
{
return (a / gcd(a, b)) * b;
}
```
# Smallest Divisor
```c++
ll smallestDivisor(ll n)
{
    // if divisible by 2
    if (n % 2 == 0)
        return 2;
 
    // iterate from 3 to sqrt(n)
    for (ll i = 3; i * i <= n; i += 2) {
        if (n % i == 0)
            return i;
    }
 
    return n;
}
```  
# Square root
```c++
  ld squareRoot(ld n)
    {
        /*We are using n itself as initial approximation
        This can definitely be improved */
        ld x = n;
        ld y = 1;
        ld e = 0.00000000001; /* e decides the accuracy level*/
        while (x - y > e) {
            x = (x + y) / 2;
            y = n / x;
        }
        return x;
    }
  ```
  # Power of Number
  ```c++
  ll power(ll a, ll b) 
  { 
ll pow = 1; 
while ( b )  
{ 
        if ( b & 1 )  
        { 
        pow = pow * a;
        // pow%=mod1;
        --b; 
        } 
        a = a*a;
        // a%=mod1; 
        b = b/2; 
} 
return pow; 
} 
```  
  
