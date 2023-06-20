#include<bits/stdc++.h>

using namespace std;

void add_from_till(vector<pair<int,int>>q,int N,int c)
{   vector<int>arr(N,0);
    
    for(int i=0;i<c;i++)
   {    
    int a=q[i].first;
    int b=q[i].second;
        
    arr[a-1]+=1;
    arr[b]-=1;
    }
   
   
   int pre[N+1],max=INT_MIN;
   pre[0]=0;

   for(int i=0;i<N;i++)
   {
    pre[i+1]=pre[i]+arr[i];
    if(max<pre[i+1])max=pre[i+1];

   }
   
   cout<<max;
   

}

int main()
{
    int c=5,N=20;
    
    
    vector<pair<int,int>>q;
    
   
    
    for(int i=0;i<c;i++)
    { int a,b;
      cin>>a>>b;

      q.push_back(make_pair(a,b));
     
    }

       
   add_from_till(q,N,c);

    return 0;
}