
#include <iostream>
using namespace std;

int GetNValue(int N)
{
    if (N <= 1) return 1;
    if (N == 2) return 2;

    return GetNValue(N-1) + GetNValue(N-2);
}

int main(int argc, char ** argv)
{
    const int N = 10;

    cout << N << ":" << GetNValue(N) << endl;

    return 0;
}
