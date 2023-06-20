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
        if((rand()%20)+5<=20)cout<<(rand()%20)+5;
        else cout<<(rand()%20)+1;
        cout<<endl;
    }
}
