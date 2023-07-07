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
# Bài 11:
```
#include<stdio.h>
#include<math.h>
int main(){
    int n;
    int sum=0;
    scanf("%d",&n);
    for(int i=1;i<=n;i++){
        sum+=pow(-1,i)*i;
    }
    printf("%d",sum);
    return 0;
}
```
# Bài 12:
```
#include<stdio.h>
#include<math.h>
int main(){
	int n;
	long long sum=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++){
		sum+=2*i;
	}
	printf("%lld",sum);
	return 0;
}
```
# Bài 14:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    long long sum=0;
    for(int i=1;i<=n;i++){
        sum+=i*i*i;
    }
    printf("%lld",sum);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 15:
```
#include<stdio.h>
#include<math.h>
int main(){
	int n;
	long long gt=1;
	scanf("%d",&n);
	for(int i=1;i<=n;i++){
		gt*=i;
	}
	printf("%lld",gt);
	return 0;
}
```
# Bài 16:
```
#include<stdio.h>
#include<math.h>
int main(){
	long long n;
	scanf("%lld",&n);
	int cnt=0;
	if(n==0){
		printf("1\n");
		return 0;
	}
	while(n>0){
		cnt++;
		n/=10;
	}
		printf("%d\n",cnt);
	
	return 0;
}
```
# Bài 17:
```
#include<stdio.h>
#include<math.h>
int main(){
    long long n;
    scanf("%lld",&n);   
    long long sum =0;
    if(n==0){
        printf("0\n");
        return 0;
    }
    while(n!= 0){
        sum += n%10 ;
        n/=10;
        
    }
        printf("%lld\n",sum);
    
    return 0;
}
```
# Bài 18:
```
#include<stdio.h>
#include<math.h>
int main(){
	long long n;
	scanf("%lld",&n);
	int cnt=0;
	if(n==0){
		printf("0\n");
		return 0;
	}
	while(n>0){
		int du=n%10;
		if(du==2||du==3||du==7||du==5){
			cnt++;
		}
		n/=10;	
		} 
		printf("%d\n",cnt);
	
	return 0;
}
```
# Bài 19:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
	int n; scanf("%d",&n);
	int kq=n/28;
	int vo = kq;
	while(vo>=3){
		int bia = vo/3;
		kq+=bia;
		vo=bia + vo%3;
		}
	printf("%d",kq);
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 20:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    if(n<=1){
        printf("-1\n");
    }
    else{
        printf("%d\n",n/2);
        if(n%2==0){
            for(int i=0;i<n/2;i++){
                printf("2 ");
            }
        }
        else{
            for(int i=0; i<n/2 -1;i++){
                printf("2 ");
            }
            printf("3 ");    
        }
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
![image](https://github.com/haridt/contest1/assets/131541155/d2c3d399-7f04-49a3-afa0-a858d79bf15c)
# Bài 21:
```
 #include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d", &n);
    for(int i=0; i<n; i++){
        for(int j=0;j<n;j++){
            printf("*");
        }
        printf("\n");
    }
    printf("\n");
    for(int i=1; i<=n; i++){
        for(int j =1;j<=n;j++){
            if(i==1 || i==n ||j==1 || j==n){
                printf("*");
            }
            else printf(" ");
        }
        printf("\n");
    }
    printf("\n");
    for(int i=1; i<=n; i++){
        for(int j =1;j<=n;j++){
            if(i==1 || i==n ||j==1 || j==n){
                printf("*");
            }
            else printf("#");
        }
        printf("\n");
    }
    printf("\n");
    for(int i=1; i<=n; i++){
        for(int j =1;j<=n;j++){
            if(i==1 || i==n || j==1 || j==n){
                printf("%d ",i);
            }
            else printf("  ");
        }
        printf("\n");
    }
    
    
    
    
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 22:
```
 #include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
	int n;
	scanf("%d", &n);
	for(int i=1; i<=n; i++){
		for(int j=1; j<=i;j++){
			printf("*");
		}
		printf("\n");
	}
	printf("\n");
	
	for(int i=n; i>=1; i--){
		for(int j=i; j>=1;j--){
			printf("*");
		}
		printf("\n");
	}
	printf("\n");
	
	for(int i=1; i<=n; i++){
		for(int j=1; j<=n-i;j++){
			printf(" ");
		}
		for(int j=1;j<=i;j++){
			printf("*");
		}
		printf("\n");
	}
	printf("\n");
	
	for(int i=1; i<=n; i++){
		for(int j=1; j<i;j++){
			printf(" ");
		}
		for(int j=i;j<=n;j++){
			printf("*");
		}
		printf("\n");
	}
	printf("\n");
	
	for( int i=1; i<=n;i++){
		for(int j=1;j<=i;j++){
			if(i ==1 || i == 2 || i==n || j==1 || j == i ){
				printf("*");
			}
			if(i >= 3 && i < n){
				if( j >= 2 && j <n){
					printf(" ");
				}
			}
		}
		printf("\n");
	}
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 23:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
	int n;
	scanf("%d",&n);
	
	for(int i=1;i<=n;i++){
		int res = i*n -(n-1);
		for(int j = 1 ; j <= n ; j++){
			printf("%d ", res);
			res++;
		}
		printf("\n");
	}
	printf("\n");
	
	//
		for(int i=0;i<n;i++){
		int res = i +1 ;
		for(int j = 1 ; j <= n ; j++){
			printf("%d ", res);
			res++;
		}
		
		printf("\n");
	}
		printf("\n");
	
	for(int i=1;i<=n;i++){
		for(int j=1;j<=n-i;j++){
			printf("~");
		}
		for(int j=n-i;j<n;j++){
			printf("%d",i);
		}
		printf("\n");
	}
		printf("\n");
	
	for(int i=1;i<=n;i++){
		int res = i;
		int dem = n -1 ;
		for(int j=1;j<=i;j++){
			printf("%d ",res);
			
			res +=dem;
			dem--;
		}
		printf("\n");
	}
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 24:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
	long long a,b; scanf("%lld%lld",&a,&b);
	long long min = fmin(a,b);
	long long gt=1;
	for(int i=1;i<=min;i++){
		gt*=i;
	}
	printf("%lld",gt);
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 25:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
	int n; scanf("%d",&n);
	int gt=1;
	double sum=1;
	for(int i=1;i<n;i++){
		gt*=i;
		sum+=1.0/gt;
	}
	printf("%.4lf",sum);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 26:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>



int main(){

    int a,b,kt,n;
    
    scanf("%d%d%d",&a,&b,&n);
    for(int x=0;x<=1000;x++){
        for(int y=0; y<=1000;y++){
            if(x*a +y*b == n){
                printf("YES");
                return 0;
            }


        }
    }

   
        printf("NO");
 

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 27:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    long long n;
    scanf("%lld",&n);
    
    while(n >= 10){
        int sum =0;
        while(n!=0){
           sum += n % 10;
           n /= 10;
           
  
        }
        n= sum;
        
  
                
 
        }
   printf("%lld",n);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 28:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    long long sum =0;
    for( int i=1; i<= n; i++){
        int gt =1;
        for(int j=1; j<= i; j++){
            gt *=j ;
        }
        sum +=gt;
    }
    printf("%lld",sum);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 29:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int x,n;
    scanf("%d\n",&n);
    long long sum = 0;
    for(int i=0; i<n;i++){
        scanf("%d",&x);
        if(x %2==0){
            sum += x ;
        }
    }
    printf("%lld", sum);
    
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 30:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int x,n; scanf("%d",&n);
    while(n--){
      scanf("%d",&x);
        if( x%2== 0){
            printf("EVEN\n");
        }
        else{
            printf("ODD\n");
        }
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
![image](https://github.com/haridt/contest1/assets/131541155/9ff94fdb-97a9-420f-a95c-791b954393dc)

# Bài 31:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n; scanf("%d",&n);
    double sum =1;
    for(int i= 1;i<=n; i++){
        int gt =1;
        for(int j =1;j <=i;j++){
            gt *= j;
        }
        sum += 1.0/gt;
    }
    printf("%.2lf",sum);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 32:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int x=65;
    int n; scanf("%d",&n);
    for(int i =1; i<=n; i++){
        for(int j=1;j<=i;j++){
            printf("%c ", x);
  
        }
        printf("\n");
        x++;
    }
 
    /* Enter your code hee. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 33:
```#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n ;
    scanf("%d",&n);
    for(int i=1;i<=n;i++){
        for(int j =1; j<=n-i;j++){
            printf("  ");
        }
        for(int x =1;x<=i*2 -1 ;x++){
            printf("* ");


        }
        printf("\n");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 35:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n; scanf("%d",&n);
    for(int i =1;i<=n;i++){
        for(int j=i-1;j>0;j--){
            printf("  ");
        }
        for(int j=2*n-(2*i-1);j>0;j--){
            printf("* ");
        }
        printf("\n");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 36:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n; scanf("%d",&n);
    for(int i =1;i<=n;i++){
        for(int j=1;j<=n-i;j++){
            printf("  ");
        }
        for(int j=1;j<i*2;j++){
            printf("* ");
        }
        printf("\n");
    }
    for(int i=2;i<=n;i++){
        for(int j=1;j<=i-1;j++){
            printf("  ");
        }
        for(int j=2*n-(2*i-1);j>0;j--){
            printf("* ");
        }
        printf("\n");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 37:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n; scanf("%d",&n);
    for(int i=1;i<=n;i++){
        for(int j=1;j<=n;j++){
            if( i==j || j== n+1-i){
                printf("%d ",i);
            }
            else{
                printf("  ");
            }
        }
        printf("\n");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 38: 
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n; scanf("%d",&n);
    for(int i=1; i<=n;i++){
        
        for(int j=1;j<=n;j++){
            if((i%2==0 && j%2==0)|| (i%2 != 0 && j%2 != 0)){
                printf("0");
            }
            else{
               printf("1");
                }
        }
        printf("\n");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 39:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n,x=65,y=98;
    scanf("%d",&n);
    for(int i=1;i<=n;i++){
        if(i%2 != 0){
            for(int j=1;j<=n;j++){
                printf("%c",x);
                x++;
            }
        }
        else{
            for(int j=1;j<=n;j++){
                printf("%c",y);
                y++;
            }
        }
        if(i %2 != 0 && i >= 1){
            x -=n-2;
        }
        else if(i%2 ==0 && y>=2){
            y-=n-2;
        }
        printf("\n");
    }
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 40:
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    for(int i=1;i<=n;i++){
        for(int j=1;j<=10;j++){
            printf("%d x %d = %d\n",i,j,i*j);
        }
        
        
        
        printf("\n");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
![image](https://github.com/haridt/contest1/assets/131541155/10ffb7d1-03a5-45b8-984c-fe05701eba11)





