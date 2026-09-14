#include<iostream>
#include<vector>
using namespace std;
main(){
    int n;
    cout<<"Nhap so luong day so :";
    cin>> n;
    vector<int> v(n);
    for(int i = 0; i < n; i++){
        cout<<"Nhap lan luot cac gia tri: ";
        cin>>v[i];
    }
    int luachonsapxep;
    cout<<"Bam phim 1 de lua chon sap xep theo chieu giam dan: \n ";
    cout<<"Bam phim 2 de lua chon sap xep theo chieu tang dan: \n ";
    cin>>luachonsapxep;
    for(int i = 0; i<n; i++){
        for(int j = i +1; j<n; j++){
            if(luachonsapxep==1){
            if(v[i] < v[j]){
                int tam =v[i];
                v[i]=v[j];
                v[j]=tam;
            }
        }
        else if(luachonsapxep==2){
            if(v[i] > v[j]){
                int tam = v[i];
                v[i]=v[j];
                v[j]=tam;
            }
        } 
    }
    }
    cout << "\n-> Vector sau khi sap xep la: ";
    for(int i = 0; i < n; i++) {
        cout << v[i] << " ";
    }
    return 0;

}
