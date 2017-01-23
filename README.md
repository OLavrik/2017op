#include <iostream>
using namespace std;

int main() {
	string s;
	cin >>s;
	int len=s.length();
	int n=0;
	int j,i,t;
	int a[7][7*len];
	for (i=0; i<7; i++){
		for (j=0; j<len*7; j++){
			a[i][j]=0;
		}
	}
	for (t=0; t<len; t++){
		if (s[t]=='A'){
			for (i=0; i<7; i++){                  
				if (i==0){
					a[i][n+3]=1;	
				}
				if (i==1){
					a[i][n+2]=1;
            		a[i][n+4]=1;
				}
				if (i==2){
					a[i][n+1]=1;
					a[i][n+5]=1;
				}
				if (i==3){
					for (j=n; j<n+7; j++){
                        a[i][j]=1;
                        
            		}  
				}
				if (i==4){
					a[i][n]=1;
            		a[i][n+6]=1;
				}
				if (i==5){
					a[i][n]=1;
            		a[i][n+6]=1;
				}
				if (i==6){
					a[i][n]=1;
            		a[i][n+6]=1;
				}
		
			}
		}
		if (s[t]=='B'){
			for (i=0; i<7; i++){                        
				if (i==0){
					for (j=n; j<n+5; j++){
                        a[i][j]=2;
                        
					}  	
				}
				if (i==1){
					a[i][n]=2;
            		a[i][n+5]=2;
				}
				if (i==2){
					for (j=n; j<n+5; j++){
                        	a[i][j]=2;
                        
					} 
				}
				if (i==3){
					for (j=n; j<n+5; j++){
                        			a[i][j]=2;
                        
            				}  
				}
				if (i==4){
					a[i][n]=2;
            				a[i][n+5]=2;
				}
				if (i==5){
					a[i][n]=2;
            				a[i][n+5]=2;
				}
				if (i==6){
					for (j=n; j<n+5; j++){
                        			a[i][j]=2;
                        
            				} 
				}
			}
			

		}
		if (s[t]=='C'){
			for (i=0; i<7; i++){                        
				if (i==0){
					for (j=n+1; j<n+5; j++){
                        a[i][j]=3;
                        
            		}  	
				}
				if (i==1){
					a[i][n]=3;
        			 a[i][n+5]=3;
				}
				if (i==2){
					a[i][n]=3;
				}
				if (i==3){
					a[i][n]=3;  
				}
				if (i==4){
					a[i][n]=3;
				}
				if (i==5){
					a[i][n]=3;
					a[i][n+5]=3;
				}
				if (i==6){
					for (j=n+1; j<n+6; j++){
                        a[i][j]=3;
                        
            		} 
				}
			}
		}
		if (s[t]=='D'){
			for (i=0; i<7; i++){                        
				if (i==0){
					for (j=n; j<n+4; j++){
                        a[i][j]=4;
                        
            		}  	
				}
				if (i==1){
					a[i][n]=4;
        			 a[i][n+5]=4;
				}
				if (i==2){
					a[i][n]=4;
					a[i][n+5]=4;
				}
				if (i==3){
					a[i][n]=4;
					a[i][n+5]=4;  
				}
				if (i==4){
					a[i][n]=4;
					a[i][n+5]=4;
				}
				if (i==5){
					a[i][n]=4;
					a[i][n+5]=4;
				}
				if (i==6){
					for (j=n; j<n+4; j++){
                        a[i][j]=4;
                        
            		} 
				}
			}
		}
		if (s[t]=='E'){
			for (i=0; i<7; i++){                        
				if (i==0){
					for (j=n; j<n+5; j++){
                        a[i][j]=5;
                        
            		}  	
				}
				if (i==1){
					a[i][n]=5;
        			 
				}
				if (i==2){
					a[i][n]=5;
					
				}
				if (i==3){
					for (j=n; j<n+5; j++){
                        a[i][j]=5;
                        
            		}
				}
				if (i==4){
					a[i][n]=5;
					
				}
				if (i==5){
					a[i][n]=5;
				}
				if (i==6){
					for (j=n; j<n+5; j++){
                        a[i][j]=5;
                        
            		} 
				}
			}
		}
		if (s[t]=='F'){
			for (i=0; i<7; i++){                        
				if (i==0){
					for (j=n; j<n+6; j++){
                        a[i][j]=6;
                        
            		}  	
				}
				if (i==1){
					a[i][n]=6;
        			 
				}
				if (i==2){
					a[i][n]=6;
					
				}
				if (i==3){
					for (j=n; j<n+3; j++){
                        a[i][j]=6;
                        
            		}
				}
				if (i==4){
					a[i][n]=6;
					
				}
				if (i==5){
					a[i][n]=6;
				}
				if (i==6){
					a[i][n]=6;
				}
			}
		}
		if (s[t]=='G'){
			for (i=0; i<7; i++){                        
				if (i==0){
					for (j=n+1; j<n+5; j++){
                        a[i][j]=7;
                        
            		}  	
				}
				if (i==1){
					a[i][n]=3;
        			 a[i][n+5]=7;
				}
				if (i==2){
					a[i][n]=7;
				}
				if (i==3){
					a[i][n]=7;  
				}
				if (i==4){
					a[i][n]=7;
					for (j=n+3; j<n+6; j++){
						a[i][j]=7;
					}
				}
				if (i==5){
					a[i][n]=7;
					a[i][n+5]=7;
				}
				if (i==6){
					for (j=n+1; j<n+6; j++){
                        a[i][j]=7;
                        
            		} 
				}
			}
		}
		if (s[t]=='I'){
			for (i=0; i<7; i++){                        
				if (i==0){
					for (j=n; j<n+7; j++){
                        a[i][j]=8;
                        
            		}  	
				}
				if (i==1){
					a[i][n+3]=8;
        			
				}
				if (i==2){
					a[i][n+3]=8;
				}
				if (i==3){
					a[i][n+3]=8; 
				}
				if (i==4){
					a[i][n+3]=8;
				}
				if (i==5){
					a[i][n+3]=8;
				}
				if (i==6){
					for (j=n; j<n+7; j++){
                        a[i][j]=8;
                        
            		} 
				}
			}
		}
		if (s[t]=='H'){
			for (i=0; i<7; i++){                        
				a[i][n]=9;
				a[i][n+6]=9;
				if (i==3){
					for (j=n+1; j<n+6; j++){
						a[i][j]=9;
					}
				}	
			}
		}
		if (s[t]=='J'){
			for (i=0; i<7; i++){                        
				if (i==0){
					for (j=n+2; j<=n+7; j++){
						a[i][j]=10;
					}  	
				}
				if (1<=i<=3){
					a[i][n+5]=10;
        			
				}
				if (4<=i<=5){
					a[i][n+1]=10;
					a[i][n+5]=10;
				}
				if (i==6){
					for (i=n+2; i<i+5; i++){
						a[i][j]=10;
					} 
				}
				
			}
		}
		n=n+7;
		
	}
	for (i=0; i<7; i++){
		for (j=0; j<len*7; j++){
			if (a[i][j]==0){
				cout<< " ";
			}
			if (a[i][j]==1){
				cout <<"A";
			}
			if (a[i][j]==2){
				cout <<"B";
			}
			if (a[i][j]==3){
				cout <<"C";
			}
			if (a[i][j]==4){
				cout <<"D";
			}
			if (a[i][j]==5){
				cout <<"E";
			}
			if (a[i][j]==6){
				cout <<"F";
			}
			if (a[i][j]==7){
				cout <<"G";
			}
			if (a[i][j]==8){
				cout <<"I";
			}
			if (a[i][j]==9){
				cout <<"H";
			}
			if (a[i][j]==10){
				cout <<"J";
			}
			if (a[i][j]==11){
				cout <<"K";
			}
			if (a[i][j]==12){
				cout <<"L";
			}
			if (a[i][j]==13){
				cout <<"M";
			}
			if (a[i][j]==14){
				cout <<"N";
			}
			if (a[i][j]==15){
				cout <<"O";
			}
			if (a[i][j]==12){
				cout <<"L";
			}
		}
		cout <<endl;
	}
	
	
}
