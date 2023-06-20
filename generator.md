//# The generator

#include<bits/stdc++.h>
#include<time.h>

using namespace std;

int main()
{
    srand(time(0));
    for(int i=0;i<20;i++)
    {
        cout<<(rand()%20)+1<<" ";
        if(i%2!=0)cout<<endl;
    }
}