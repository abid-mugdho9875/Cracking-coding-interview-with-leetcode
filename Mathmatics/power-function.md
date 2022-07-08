power-function

# Modular exponentation

3^200 mod 50

1. Here we can follow can follow an pretty algorithum without calculating 3^200.

- 3^1 = 3 mod 50 = 3
- 3^2 = 9 mod 50 = 9
- 3^4 = ((3^2)^2) mod 50
  = (9^2) mod 50 = 31
- 3^8 = (31^2) mod 50 = 11

# here, it releates with the previous expression

- 3^16 = (11^2) mod 50 = 21
- 3^32 = (21^2) mod 50 = 41
- 3^64 = (41^2) mod 50 = 31
- 3^128 = (31^2) mod 50 = 11

- 3^256 here 256 is larger than 200. so it is stop position.

Binary expansion for 3^200 is 11001000 ---> 128 + 64+ 8
so, 3^200 = 3^128 . 3^64 . 3^8 = 11*31*11 mod 50 = 1


Implementation using cpp--->
// Online C++ compiler to run C++ program online
using namespace std;
int Bigmod(int base, int power, int mod){
    if (power ==0 ) return 1;
    else if (power % 2 == 1){
        int a = base % mod;
        int b = (Bigmod(base, power - 1, mod)) %mod;
        return (a * b) % mod;
    }
      else if (power % 2 == 0){
        int a = (Bigmod(base, power/2, mod)) %mod;
        return (a * a) % mod;
    }
}
int main(){
    int base, power, mod;
    cin>>base>>power>>mod;
    cout<<Bigmod(base, power, mod) <<endl;
    return 0;

}
