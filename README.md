#include<iostream>
#include<vector>
using namespace std;
int main(){
	int n;
	cout<<"Nhap so luong phan tu trong day: ";
	cin>> n;
	vector<int> v(n);
	
	for(int i = 0; i < n; i++){
		cout<<"Nhap lan luot cac phan tu trong day: ";
		cin>>v[i];
	}
	int Tong = 0;
	for(int i = 0; i < n; i++){
		Tong += v[i];
	}
	cout<<"Tong  cua day la: "<< Tong << endl;
	return 0;
}
