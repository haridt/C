# Bài 1:
```
#include<stdio.h>

int main(){
	int n;
	long long sum=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++){
		sum+=i;
	}
	printf("%lld",sum);
	
	return 0;
}
```
# Bài 2:
```
#include<stdio.h>

int main(){
	int n;
	long long sum=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++){
		sum+=1ll*i*i;
	}
	printf("%lld",sum);
	
	return 0;
}
```
# Bài 3:
```
#include<stdio.h>

int main(){
	int n;
	long long sum=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++){
		if(i%3==0){
			sum+=i;	
		}	
	}
	printf("%lld",sum);
	
	return 0;
}
```
# Bài 4:
```
#include<stdio.h>

int main(){
    int n;
    double sum=0;
    scanf("%d",&n);
    for(int i=1;i<=n;i++){
        sum+=1.0/i;
    }
    printf("%.3lf",sum);
    
    return 0;
}    
```
# Bài 6:
```
#include<stdio.h>
#include<math.h>
int main(){
	long long n;
	scanf("%lld",&n);
	long long sum=0;
	for(int i=1; i<=sqrt(n);i++){
		if(n%i==0){
			sum +=i;
			if(i!= n/i){
				sum +=n/i;
			}
			 /* uoc con lai cua i
							vd:i=2;n=60
							60%2==0 va 60/2= 20
							ta co:2 la uoc cua 60, va 20 cung la uoc cua 60
							vay trong cung 1 i ta co the tim 2 uoc cua n 
						 */
		}
	}
	printf("%lld",sum);
	return 0;
}
```
# Bài 7:
```
#include<stdio.h>
#include<math.h>
int main(){
	int n;
	scanf("%d",&n);
	int count=0;
	for(int i=1; i<=sqrt(n);i++){
		if(n%i==0){
			count ++;
			if(i!= n/i){
				int j= n/i;
				count ++;
			}
			 /* uoc con lai cua i
							vd:i=2;n=60
							60%2==0 va 60/2= 20
							ta co:2 la uoc cua 60, va 20 cung la uoc cua 60
							vay trong cung 1 i ta co the tim 2 uoc cua n 
						 */
		}
	}
	printf("%d\n",count);
	for(int i=1; i<=n;i++){
		if(n%i==0){
			printf("%d ",i);
		}
	}
	
	return 0;
}
```
# Bài 8:
```
#include<stdio.h>
#include<math.h>
int main(){
	long long n;
	scanf("%lld",&n);
	for(int i=1; i<=sqrt(n);i++){
		printf("%lld ",1ll*i*i);
	}
	
	return 0;
}
```
# Bài 9:
```
#include<stdio.h>
#include<math.h>
int main(){
	int n;
	scanf("%d",&n);
	long long tich=1;
	for(int i=1; i<=sqrt(n);i++){
		if(n%i==0){
			tich *=i*1ll;
			if(i!= n/i){
				tich *=1ll*(n/i);
			}
			 /* uoc con lai cua i
							vd:i=2;n=60
							60%2==0 va 60/2= 20
							ta co:2 la uoc cua 60, va 20 cung la uoc cua 60
							vay trong cung 1 i ta co the tim 2 uoc cua n 
						 */
		}
	}
	printf("%lld",tich);
	return 0;
}
```
# Bài 10:
```
#include<stdio.h>
#include<math.h>
int main(){
	int n;
	scanf("%d",&n);
	int check=0;
	for(int i=1;i<=n;i++){
		int so;
		scanf("%d",&so);
		if(so==2022){
			check=1;
		}
	}
	if(check==1){
		printf("YES");
	}
	else{
		printf("NO");
	}
	return 0;
}
```
![alt](https://github.com/haridt/contest1/assets/131541155/134407b2-3efd-4aeb-b5d5-3f97f011c33f)

