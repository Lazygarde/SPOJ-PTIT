#include <bits/stdc++.h>
using namespace std;
bool cmp(int a,int b){
	return a>b;
}
int main(){
	int n,x,pos1=0,pos2=0,s=0;
	cin>>n;
	vector <int> a1,a2,b1,b2;
	for(int i=0;i<n;i++){
		cin>>x;
		if(x>0) a1.push_back(x);
		else a2.push_back(x);
	}
	for(int i=0;i<n;i++){
		cin>>x;
		if(x>0) b1.push_back(x);
		else b2.push_back(x);
	}
	sort(a1.begin(),a1.end(),cmp);
	sort(b1.begin(),b1.end(),cmp);
	sort(a2.begin(),a2.end());
	sort(b2.begin(),b2.end());
	while(1){
		if(pos1==a1.size()||pos2==b2.size()) break;
		if(a1[pos1]+b2[pos2]<0){
			s++;
			pos1++;pos2++;
		}
		else{
			pos1++;
		}
	}
	pos1=0;pos2=0;
	while(1){
		if(pos1==b1.size()||pos2==a2.size()) break;
		if(b1[pos1]+a2[pos2]<0){
			s++;
			pos1++;pos2++;
		}
		else{
			pos1++;
		}
	}
	cout<<s;
}
