# Bài 1. Tính toán giá trị của biểu thức
```
#include<stdio.h>
#include<math.h>

int main(){
	int x;
	scanf("%d",&x);
	printf("%lld",1ll*x*x*x+3ll*x*x+x+1);
	return 0;
}
```
# Bài 2. Tính toán giá trị biểu thức 2
```
#include<stdio.h>

int main(){
    int a,b,c;
    scanf("%d %d %d",&a,&b,&c);
    printf("%lld",1ll*a*(b+c)+1ll*b*(a+c));
    return 0;
}

```
# Bài 3. Đổi nhiệt độ
```
#include<stdio.h>

int main(){
    short c;
    scanf("%d",&c);
    printf("%.2f",((float)c*9/5)+32    );
    return 0;
}
```
# Bài 4. Chu vi và diện tích hình tròn
```
#include<stdio.h>

int main(){
     int r;
    scanf("%d",&r);
    printf("%.4lf %.4lf",r*3.14*2,r*r*3.14);
    return 0;
}
```
# Bài 5. Khoảng cách Euclid
```
#include<stdio.h>
#include<math.h>

int main(){
    int x1,y1,x2,y2;
    scanf("%d %d %d %d",&x1,&y1,&x2,&y2);
    double dis=sqrt(pow(x1-x2,2)+pow(y1-y2,2));
    printf("%.2lf",dis);
    return 0 ;
    
}
```
#  Bài 6. Luyện tập viết câu điều kiện
```
#include<stdio.h>

int main(){
	int n;
	scanf("%d",&n);
	//1
	if(n%2==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//2
	if(n%3==0 && n%5==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//3
	if(n%3==0 && n%7!=0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//4
	if(n%3==0 || n%7==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//5
	if(n>30 && n<50){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//6
	if(n>=30 && (n%2==0 || n%3==0 || n%5==0)){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//7
	if(n>=10 && n<=99 &&(n%10==2 || n%10==3 || n%10== 5 || n%10== 7)){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//8
	if(n<=100 && n%23==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//9
	if(n<10 || n>20){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	//10
	int r=n%10;
	if(r%3==0){
		printf("YES\n");
	}
	else{
		printf("NO\n");
	}
	return 0;
}
	
```
# Bài 7. Số lớn nhất và nhỏ nhất
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main(){
    int a,b;
    scanf("%d %d",&a,&b);
    long long s1= a/b*b*1ll;
    long long s2= (a+b-1)/b*b*1ll;
    printf("%lld\n",s1);
    printf("%lld\n",s2);
    return 0;
}
```
# Bài 8. Tổng, hiệu, tích, thương
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main(){
    int a,b;
    scanf("%d %d",&a,&b);
    printf("%lld\n",(long long)a+b);
    printf("%d\n",a-b);
    printf("%lld\n",(long long)a*b);
    if(b>0){
        printf("%.4lf",(double)a/b);
    }
    else{
        printf("INVALID");
    }
    return 0;
}
```
# Bài 9.Kiểm tra năm nhuận
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    if(n%400==0 || (n%4==0 && n%100!=0)){
        printf("YES");
    } 
    else{
        printf("NO");
    }
    return 0;
}
```
# Bài 10. Tam giác hợp lệ
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a,b,c;
    scanf("%d %d %d",&a,&b,&c);
    if(a,b,c>0 && a+b>c&&a+c>b&&c+b>a){
        printf("YES");
    }   
    else{
        printf("NO");
    }
    return 0;
}
```
<img src="https://imgur.com/a/RQOVBk4">

# Bài 11. Kiểm tra tam giác
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a,b,c;
    scanf("%d %d %d",&a,&b,&c);
    if(a>0 && b>0 && c>0 && a+b>c && a+c>b && b+c>a){
        if(a==b&&b==c){
            printf("1");
        }
        else if(a==b||b==c){
            printf("2");
        }
        else if(a*a==b*b+c*c||b*b==a*a+c*c||c*c==a*a+b*b){
            printf("3");
        }
        else if(a+b>c||a+c>b||b+c>a){
            printf("4");
        }
    }
    else{
        printf("INVALID");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 12. Số ngày của tháng
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int t,n;
    scanf("%d %d",&t,&n);
    if(t>0&& t<13  && n>0){
        if(n%400==0||(n%4==0&&n%100!=0)){
            if(t==2){
                printf("29");
            }
            else if(t==1||t==3||t==5||t==7||t==8||t==10||t==12){
            printf("31");
            }
            else{
                printf("30");
            }
        }
        else if(t==1||t==3||t==5||t==7||t==8||t==10||t==12){
            printf("31");
        }
        else if(t==2){
            printf("28");
        }
        else{
            printf("30");
        }
        
    }else{
        printf("INVALID");
    }
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 13. Đổi ngày sang năm, tuần, ngày
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    int nam=n/365;
    n=n%365;
    int tuan=n/7;
    int ngay =n%7;
    printf("%d %d %d",nam,tuan,ngay);
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
#  Bài 14. Xếp loại học sinh
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    float a,b,c,d;
    scanf("%f %f %f %f",&a,&b,&c,&d);
    float tb=(a+b+c*2+d*3)/7;
    if( tb>=8){
        printf("GIOI");
    }
    else if(6.5<=tb){
        printf("KHA");
    }
    else if(5<=tb){
        printf("TRUNG BINH");
    }
    else{
        printf("YEU");
    }
    
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 15. Mua nước
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    long long n,a,b;
    scanf("%lld %lld %lld",&n,&a,&b);
    if(a*2<=b){
        printf("%lld",n*a);
    }
    else{
        if(n%2==0){
            printf("%lld",n/2*b);
        }
        else{
            printf("%lld",n/2*b+a);
        }
    }
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 16. Kí tự kế tiếp
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int kitu;
    scanf("%c",&kitu);
    if(kitu=='Z'||kitu=='z'){
        printf("a");
    }
    else if(kitu>='A'&&kitu<'Z'){
        printf("%c",kitu+33);
    }
    else if('a'<=kitu&& kitu<'z'){
        printf("%c",kitu+1);
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 17. Kiểm tra chữ cái
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int kitu;
    scanf("%c",&kitu);
    if(kitu>='A'&&kitu<='Z'){
        printf("UPPER");
    }
    else if(kitu>='a'&&kitu<='z'){
        printf("LOWER");
    }
    else if(kitu>='0'&&kitu<='9'){
        printf("DIGIT");
    }
    else{
        printf("SPECIAL");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 18. Chuyển đổi in hoa in thường
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>
char swap(char c){
    if(c>='A'&&c<='Z'){
     c=c+32;
    }
    else if(c>='a'&&c<='z'){
    c-=32;
    }
    else c;
    return c;
}

int main() {
    int kitu;
    scanf("%c",&kitu);
    printf("%c",swap(kitu));

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 19. Domino
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int m,n;
    scanf("%d %d",&m,&n);
    if(m%2==0){
        long long domino= 1ll*(m/2)*n;
        printf("%lld",domino);
    }
    else{
        long long domino= 1ll*((m-1)/2)*n+(n/2);
        printf("%lld",domino);
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 20. Lát đá quảng trường
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int m,n,a;
    scanf("%d %d %d",&m,&n,&a);
    int ngang,doc;
    if(m%a==0){
        doc=m/a;
    }
    else doc=m/a +1;
    if(n%a==0){
        ngang=n/a;
    }
    else ngang=n/a+1;
    printf("%lld",1ll*doc*ngang);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 21. Frog
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a,b,k;
    scanf("%d %d %d",&a,&b,&k);
    if(k%2==0){
        long long p=k/2*1ll*a;
        long long t=k/2*1ll*b;
        printf("%lld",p-t);
    }
    else{
        long long p= (k/2+1)*1ll*a;
        long long t=k/2*1ll*b;
        printf("%lld",p-t);
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 22. Đồng xu
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    long long n,s;
    scanf("%lld %lld",&n,&s);
    if(s%n==0){
        printf("%lld",s/n);
    }
    else{
        printf("%lld",s/n +1);
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
#  Bài 23. Doremon leo cầu thang
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n,m;
    scanf("%d %d",&n,&m);
    int min, max=n;
    if(n%2==0){
        min= n/2;
    }
    else{
        min=n/2+1;
    }
    int ketqua=((min+m-1)/m) *m;
    if(ketqua<=max){
        printf("%d",ketqua);
    }
    else{
        printf("-1");
    }
    
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 24. Đường đi ngắn nhất
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int d1,d2,d3;
    scanf("%d %d %d",&d1,&d2,&d3);
    int s1=d1+d3+d2;
    int s2=d1*2+d2*2;
    int s3=d1+d3+d3+d1;
    int s4=2*(d2+d3);
    printf("%d",(int)fmin(fmin(s1,s2), fmin(s3,s4)));
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 25. Đổi tiền
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    int res=0;
    res+=n/100; n=n%100;
    res+=n/20; n=n%20;
    res+=n/10; n=n%10;
    res+=n/5; n=n%5;
    res+=n;
    printf("%d", res);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 26. Số lớn nhất nhỏ nhất trong 4 số
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    long long a,b,c,d;
    scanf("%lld %lld %lld %lld",&a,&b,&c,&d);
    long long min=a, max=a;
    if(b<min) min=b;
    if(c<min) min=c;
    if(d<min) min=d;
    if(b>max) max=b;
    if(c>max) max=c;
    if(d>max) max=d;
    printf("%lld %lld",max,min);
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 27. Làm tròn số
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    double a;
    scanf("%lf",&a);
    printf("%d",(int)round(a));
 
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 28. Cấp số cộng
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n,u1,d;
    scanf("%d %d %d",&n,&u1,&d);
    long long un=u1+1ll*(n-1)*d;
    long long S=n*(u1+un)/2;
    printf("%lld",S);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}

```
# Bài 29. Cấp số nhân
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a,b,c,d;
    scanf("%d %d %d %d",&a,&b,&c,&d);
    if(b%a==0){
        int x=b/a;
        b*=x;
        if(b==c){
            c*=x;
            if(c==d){
                printf("YES");
            }
        }
    }else{
        printf("NO");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 30. Tổ hợp chập 2
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int n;
    scanf("%d",&n);
    printf("%lld",1ll*n*(n-1)/2);

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
#  Bài 31. Bizon the Champion
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a1,a2,a3,b1,b2,b3,n;
    scanf("%d %d %d %d %d %d %d",&a1,&a2,&a3,&b1,&b2,&b3,&n);
    int x=(int)ceil(((double)a1+a2+a3)/5);
    int y=(int)ceil(((double)b1+b2+b3)/10);
    int res= x+y;
    if(res<=n){
        printf("YES");
    }
    else{
        printf("NO");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 32. Ghép số
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int k2,k3,k5,k6;
    scanf("%d %d %d %d",&k2,&k3,&k5,&k6);
    int x=fmin(k2,fmin(k6,k5));
    if(x==k2){
        printf("%lld",x*256ll);
    }
    else{
        if((k2-x)<k3){
            printf("%lld",256ll*x+32ll*(k2-x));
        }else{
            printf("%lld",256ll*x+32ll*k3);
        }
    }
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
#  Bài 33. Chia tiền
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int a,b,c,n;
    scanf("%d %d %d %d",&a,&b,&c,&n);
    int tong=a+b+c+n;
    if(tong%3==0){
        int res=tong/3;
        if(res>=a&&res>=b&&res>=c){
            printf("YES");
        }
        else printf("NO");
    }
    else printf("NO");

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# Bài 34. Sự hào phóng
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int c1,c2,c3,c4,c5;
    scanf("%d %d %d %d %d",&c1,&c2,&c3,&c4,&c5);
    int tong= c1+c2+c3+c4+c5;
    if(tong%5==0){
        int b=tong/5;
        if(b!=0){
            printf("%d",b);
        }
        else{
            printf("-1");
        }
    }else{
        printf("-1");
    }
    

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
#  Bài 35. HPNY
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int h,m;
    scanf("%d %d",&h,&m);
    int res= 24*60;
    printf("%d",res-(h*60+m));

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
# [C++ Test 1]. Problem E
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    double a,b,c;
    scanf("%lf %lf %lf",&a,&b,&c);
    if(a==0&&b==0&&c==0){
        printf("VO SO NGHIEM");
    }
    else if(a==0&&b==0&&c!=0){
        printf("VO NGHIEM");
    }
    else if(a==0){
        printf("%.2lf",-c/b);
    }
    else{
        double delta=b*b-4*a*c;
        if(delta<0) printf("VO NGHIEM");
        else if(delta==0) printf("%.2lf",-b/(2*a));
        else{
            double x1=(-b-sqrt(delta))/(2*a);
            double x2=(-b+sqrt(delta))/(2*a);
            printf("%.2lf %.2lf",fmin(x1,x2), fmax(x1,x2));
        }
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```
