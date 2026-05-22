# Patterns
Patterns with code

## Index

- [Pattern 1 - Grid Pattern](#pattern-1)
- [Pattern 2 - Number Triangle](#pattern-2)
- [Pattern 3 - Diagonal Box](#pattern-3)
- [Pattern 4 - Z Pattern](#pattern-4)
- [Pattern 5 - Growing Blocks](#pattern-5)
- [Pattern 6 - Expanding Lines](#pattern-6)
- [Pattern 7 - Hollow Pyramid](#pattern-7)
- [Pattern 8 - Hollow Number Triangle](#pattern-8)
- [Pattern 9 - Number Diamond](#pattern-9)
- [Pattern 10 - Left Arrow Pattern](#pattern-10)
- [Pattern 11 - Double Pyramid](#pattern-11)
- [Pattern 12 - X Number Pattern](#pattern-12)
- [Pattern 13 - Hollow Diamond](#pattern-13)
- [Pattern 14 - Number Block Pattern](#pattern-14)
- [Pattern 15 - Alphabet Number Pattern](#pattern-15)
- [Pattern 16 - Multiplication Triangle](#pattern-16)
- [Pattern 17 - Mirror Number Pattern](#pattern-17)
- [Pattern 18 - Diamond Star Pattern](#pattern-18)
- [Pattern 19 - X Box Pattern](#pattern-19)
- [Pattern 20 - Mixed Number Pattern](#pattern-20)
- [Pattern 21 - Reverse Mirror Numbers](#pattern-21)
- [Pattern 22 - Vertical Star Blocks](#pattern-22)
- [Pattern 23 - Triple Star Pattern](#pattern-23)
- [Pattern 24 - Binary Reverse Triangle](#pattern-24)
- [Pattern 25 - Palindrome Number Pyramid](#pattern-25)
- [Pattern 26 - Number and Star Mirror](#pattern-26)
- [Pattern 27 - Reverse Number and Star Mirror](#pattern-27)
- [Pattern 28 - Odd Number Triangle](#pattern-28)
- [Pattern 29 - Reverse Star Ladder](#pattern-29)
- [Pattern 30 - Expanding Star Blocks](#pattern-30)
- [Pattern 31 - Multiplication Series Pattern](#pattern-31)

---

## Pattern 1 
<p align="right"> [🔝 Back to Index](#index) </p>

```c
0|0  0|1  0|2  0|3  0|4

1|0  1|1  1|2  1|3  1|4

2|0  2|1  2|2  2|3  2|4

3|0  3|1  3|2  3|3  3|4

4|0  4|1  4|2  4|3  4|4
```
<p>This Grid pattern to understand the cound of grid of </p>

<details>

<summary> 👉 Click to view the Code of Pattern 1 </summary>

```c
#include<stdio.h>
int main(void){

    int i, j, row=5;

    for(i=0; i<row; i++){
        for(j=0; j<row; j++)
            printf("%d|%d  ", i, j);
        printf("\n\n");
    }
}
```

</details>

---
## Pattern 2 <p align="right"> [🔝 Back to Index](#index) </p>
```c
50 
45 40 
35 30 25 
20 15 10 5 
```

<details>
<summary> 👉 Click to view the Code of Pattern 2 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,k=50,n=4;
        for(i=1;i<=n;i++){
            for(j=0;j<i;j++){
                printf("%d ",k);
                k=k-5;
            }
            printf("\n");
        }
}
```
</details>

---

## Pattern 3 <p align="right"> [🔝 Back to Index](#index) </p>
```c
*       * 
* *     * 
*   *   * 
*     * * 
*       * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 3 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,n=5;
    for(i=0;i<n;i++){
        for(j=0;j<n;j++){
            if(j==0||j==n-1||i==j){
                printf("* ");
                }
            else{
                printf("  ");
            }
        }
        printf("\n");

    }
}
```
</details>

---

## Pattern 4 <p align="right"> [🔝 Back to Index](#index) </p>

```c
* * * * * 
      *   
    *     
  *       
* * * * * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 4 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,n=5;
    for(i=0;i<n;i++){
        for(j=0;j<n;j++){
                if(i==0||i==n-1||n==i+j+1){
                printf("* ");
            }
            else{
                printf("  ");
            }
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 5 <p align="right"> [🔝 Back to Index](#index) </p>

```c
* * 
*
*
*
* * * * 
* * * * 
*
*
*
* * * * * * 
* * * * * * 
* * * * * * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 5 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,k,n=3;
    for(i=1;i<=n;i++){
        for(k=0;k<i;k++){
            for(j=0;j<2*i;j++){
                printf("* ");
            }
            printf("\n");
        }
        if(i==n){
            break;
        }
        for(k=0;k<3;k++){
            printf("*\n");
        }
    }
}
```
</details>

---

## Pattern 6 <p align="right"> [🔝 Back to Index](#index) </p>

```c
* * * 
* * * 
*
* * * * * * 
* * * * * * 
*
*
* * * * * * * * * 
* * * * * * * * * 
```
---

<details>
<summary> 👉 Click to view the Code of Pattern 6 </summary>

```c
#include<stdio.h>

int main(void){
int i,j,k,n=3;
    for(i=1;i<=n;i++){
        for(j=0;j<2;j++){
            for(k=0;k<3*i;k++){
                printf("* ");
            }
            printf("\n");
        }
        if(i==n){
            break;
        }
        for(j=0;j<i;j++){
            printf("*\n");
        }
    }

}
```
---

</details>

## Pattern 7 <p align="right"> [🔝 Back to Index](#index) </p>

```c
      *
     * *
    *   *
   *     *
  *       *
 ***********
```
<details>
<summary> 👉 Click to view the Code of Pattern 7 </summary>
---

```c
#include<stdio.h>

int main(void){
    int i,j,k,n=6;
    for(i=0;i<n;i++){
        for(k=0;k<n-i;k++){
        printf(" ");
        }
        for(j=0;j<2*i+1;j++){
            if(j==0||j==2*i||i==n-1){
                printf("*");
            }
            else{
                printf(" ");
            }
        }
        printf("\n");
    }
}
```
</details>

---
## Pattern 8 <p align="right"> [🔝 Back to Index](#index) </p>

```c
1 
1 2 
1   3 
1     4 
1 2 3 4 5 
```
<details>
<summary> 👉 Click to view the Code of Pattern 8 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,n=5;
    for(i=1;i<=n;i++){
        for(j=1;j<=i;j++){
            if(j==1||j==i||i==n){
                printf("%d ",j);
            }
            else{
                printf("  ");
            }
        }
        printf("\n");
    }

}
```
</details>

---
## Pattern 9 <p align="right"> [🔝 Back to Index](#index) </p>

```c
          1 
        1 2 3 
      1 2 3 4 5 
    1 2 3 4 5 6 7 
  1 2 3 4 5 6 7 8 9 
    1 2 3 4 5 6 7 
      1 2 3 4 5 
        1 2 3 
          1 
```
<details>
<summary> 👉 Click to view the Code of Pattern 9 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,k,n=4,f;
    for(i=-n;i<=n;i++){
        if(i<0){
        k=-i;
        }
        else{
            k=i;
        }
        for(j=0;j<k+1;j++){
            printf("  ");
        }
        for(j=0,f=1;j<(n-k)*2+1;f++,j++){
            printf("%d ",f);
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 10 

<p align="right"> [🔝 Back to Index](#index) </p>

```c
 * * * * * 
  * * * * 
   * * * 
    * * 
     * 
    * * 
   * * * 
  * * * * 
 * * * * * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 10 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,f,n=4;
    for(i=-n;i<=n;i++){
        if(i<0){
            f=-i;
        }
        else{
            f=i;
        }
        for(j=0;j<n+1-f;j++){
            printf(" ");
        }
        for(j=0;j<f+1;j++){
            printf("* ");
        }
        printf("\n");
    }
}
```
</details>

---


## Pattern 11 <p align="right"> [🔝 Back to Index](#index) </p>

```c
*                         * 
                          
* * *                 * * * 
                        
* * * * *         * * * * * 
                      
* * * * * * * * * * * * * * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 11 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,n=8;
    for(i=1;i<n;i++){
        for(j=0;j<i;j++){
            if(i%2!=0){
                printf("* ");
            }
            else{
                printf("  ");
            }
        }
        for(j=i;j<n-1;j++){
            printf("    ");
        }
        for(j=0;j<i;j++){
            if(i%2!=0){
                printf("* ");
            }
            else{
                printf(" ");
            }
        }
        printf("\n");
    }
}
```
</details>

---


## Pattern 12 <p align="right"> [🔝 Back to Index](#index) </p>

```c
1        1 
 2      2  
  3    3   
   4  4    
    5     
   4  4    
  3    3   
 2      2  
1        1 
```
<details>
<summary> 👉 Click to view the Code of Pattern 12 </summary>

```c
#include<stdio.h>

int main(void){
    int i,j,n=9;
    for(i=0;i<n;i++){
        for(j=0;j<n;j++){
            if(i==j||n==i+j+1){
                if(i==j){
                    if(i<n/2){
                        printf("%d ",i+1);
                    }
                    else{
                        printf("%d ",n-i);
                    }
                }
                else if(n==i+j+1){
                    if(i<n/2){
                        printf("%d ",i+1);
                    }
                    else{
                        printf("%d ",j+1);
                    }
                }
            }
            else{
                printf(" ");
            }
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 13 <p align="right"> [🔝 Back to Index](#index) </p>

```c
    *
   * *
  *   *
 *     *
*       *
 *     *
  *   *
   * *
    *
```

<details>
<summary> 👉 Click to view the Code of Pattern 13</summary>

#### Pattern 13 (Method 1)

```c

#include <stdio.h>
int main(void){
    int i,j,k,n=5,star=1,space=n-1;
    for(i=1;i<=2*n;i++){
        for(j=1;j<=space;j++){
            printf(" ");
        }
        for(k=1;k<=2*star-1;k++){
            if(k==1||k==2*star-1){
            printf("*");
            }
            else{
            printf(" ");
            }
        }
        if(i<n){
            star++;
            space--;
        }
        else{
            star--;
            space++;
        }
        printf("\n");
    }
}
```

## Or
#### Pattern 13 (Method 2)
```c
#include <stdio.h>

int main(void) {
    int rows = 5;
    int spaces;

    for (int i = 1; i <= rows; i++) {
        for (spaces = 1; spaces <= rows - i; spaces++) {
            printf(" ");
        }
        printf("*");
        if (i != 1) {
            for (spaces = 1; spaces <= (2 * i - 3); spaces++) {
                printf(" ");
            }
            printf("*");
        }

        printf("\n");
    }
    for (int i = rows - 1; i >= 1; i--) {
        for (spaces = 1; spaces <= rows - i; spaces++) {
            printf(" ");
        }
        printf("*");
        if (i != 1) {
            for (spaces = 1; spaces <= (2 * i - 3); spaces++) {
                printf(" ");
            }
            printf("*");
        }
        printf("\n");
    }
}
```

</details>

---

## Pattern 14 <p align="right"> [🔝 Back to Index](#index) </p>

```c
1 1 1 1 1 1 
1 1 1 1 2 2 
1 1 1 3 3 3 
1 1 4 4 4 4 
1 5 5 5 5 5 
6 6 6 6 6 6 
```
<details>
<summary> 👉 Click to view the Code of Pattern 14 </summary>

```c
#include <stdio.h>
int main(void){
    int i,j,n=6;
    for(i=1;i<=n;i++){
        for(j=0;j<n-i;j++){
            printf("1 ");
        }
        for(j=0;j<i;j++){
            printf("%d ",i);
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 15 <p align="right"> [🔝 Back to Index](#index) </p>

```c
A 
1 1 
B B B 
2 2 2 2 
C C C C C 
3 3 3 3 3 3 
D D D D D D D 
```
<details>
<summary> 👉 Click to view the Code of Pattern 15 </summary>

```c
#include <stdio.h>
int main(void){
    int i,j,n=7;
    for(i=1;i<=n;i++){
        for(j=0;j<i;j++){
            if(i%2!=0){
                printf("%c ",65+i/2);
            }
            else{
                printf("%d ",i/2);
            }
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 16 <p align="right"> [🔝 Back to Index](#index) </p>

```c
 1 2 3 4 5 
  2 4 6 8 
   3 6 9 
    4 8 
     5 
```
<details>
<summary> 👉 Click to view the Code of Pattern 16 </summary>

```c
#include <stdio.h>
int main(void){
    int i,j,n=6;
    for(i=1;i<=n;i++){
        for(j=0;j<i;j++){
            printf(" ");
        }
        for(j=1;j<=n-i;j++){
            printf("%d ",i*j);
        }
        printf("\n");
    }
}
```
</details>

---


## Pattern 17 <p align="right"> [🔝 Back to Index](#index) </p>


```c

1 1 
1 2 2 1 
1 2 3 3 2 1 
1 2 3 4 4 3 2 1 
1 2 3 4 5 5 4 3 2 1 
1 2 3 4 5 6 6 5 4 3 2 1 
```

<details>

<summary> 👉 Click to view the Code of Pattern 17 </summary>


```c

#include <stdio.h>
int main(void){
    int i,j,n=6;
    for(i=1;i<=n;i++){
        for(j=1;j<=i;j++){
            printf("%d ",j);
        }
        for(j=i;j>0;j--){
            printf("%d ",j);
        }
        printf("\n");
    }
}
```

</details>

---

## Pattern 18 <p align="right"> [🔝 Back to Index](#index) </p>

```c
     * 
    * * 
   * * * 
  * * * * 
 * * * * * 
  * * * * 
   * * * 
    * * 
     * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 18 </summary>

```c
#include <stdio.h>

int main(void) {

    int i, j, k, n = 4;

    for(i = -n; i <= n; i++) {
        if(i < 0)
            k = -i;else 
            k = i;
        for(j = 0; j < k + 1; j++)
            printf(" ");
        
        for(j = 0; j <= n - k; j++)
            printf("* ");
        
        printf("\n");
    }
}
```
</details>

---

## Pattern 19 <p align="right"> [🔝 Back to Index](#index) </p>


```c

* * * * * * * 
* *       * * 
*   *   *   * 
*     *     * 
*   *   *   * 
* *       * * 
* * * * * * *
```

<details>

<summary> 👉 Click to view the Code of Pattern 19 </summary>


```c
#include <stdio.h>

int main(void) {
    int i, j, n=7;
    for(i=0;i<n;i++){
        for(j=0;j<n;j++){
            if(i==0||i==n-1||j==0||j==n-1||i==j||n==i+j+1)
                printf("* ");else
                printf("  ");
        }
        printf("\n");
    }
}
```

</details>

---




## Pattern 20 <p align="right"> [🔝 Back to Index](#index) </p>

```c
1 
2 * 
3 * 9 
4 * 12 * 
5 * 15 * 25 
6 * 18 * 30 * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 20 </summary>

```c
#include <stdio.h>

int main(void) {
    int i,j,k,n=5;
    for(i=0;i<=n;i++){
        for(j=0;j<=i;j++){
            if(j%2==0)
            printf("%d ",(i+1)*(j+1));else
            printf("* ");
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 21 <p align="right"> [🔝 Back to Index](#index) </p>

```c
1 2 3 4 5 4 3 2 1 
1 2 3 4 3 2 1 
1 2 3 2 1 
1 2 1 
1 
```
<details>
<summary> 👉 Click to view the Code of Pattern  </summary>

```c
#include <stdio.h>

int main(void) {
    int i,j,n=5;
    for(i=n;i>0;i--){
        for(j=1;j<=i;j++){
            printf("%d ",j);
        }
        for(j=i-1;j>0;j--){
            printf("%d ",j);
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 22 <p align="right"> [🔝 Back to Index](#index) </p>

```c
*
* * 
*
*
*
* * * * 
*
*
*
*
*
* * * * * * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 22 </summary>

```c
#include <stdio.h>

int main(void) {
int i,j,n=3;
    for(i=1;i<=n;i++){
        for(j=0;j<i*2-1;j++){
            printf("*\n");
        }
        for(j=0;j<i*2;j++){
            printf("* ");
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 23 <p align="right"> [🔝 Back to Index](#index) </p>

```c
*
* * * 
*
* * * 
* * * 
*
* * * 
* * * 
* * * 
*
* * * 
* * * 
* * * 
* * * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 23 </summary>

```c
#include <stdio.h>

int main(void) {
    int i,j,k,n=4;
    for(i=1;i<=n;i++){
        printf("*\n");
        for(j=0;j<i;j++){
            for(k=0;k<3;k++){
                printf("* ");
            }
            printf("\n");
        }
    }
}
```
</details>

---


## Pattern 24 <p align="right"> [🔝 Back to Index](#index) </p>


```c

0 1 0 1 0 1 
1 0 1 0 1 
0 1 0 1 
1 0 1 
0 1
```

<details>

<summary> 👉 Click to view the Code of Pattern 24 </summary>


```c

#include <stdio.h>

int main(void) {
    int i,j,n=5;
    for(i=0;i<n;i++){
        for(j=i;j<=n;j++){
            printf("%d ",j%2);
        }
        printf("\n");
    }
}
```

</details>

---


## Pattern 25 <p align="right"> [🔝 Back to Index](#index) </p>


```c

1 
1 2 1 
1 2 3 2 1 
1 2 3 4 3 2 1 
1 2 3 4 5 4 3 2 1 
```

<details>

<summary> 👉 Click to view the Code of Pattern 25 </summary>


```c

#include <stdio.h>

int main(void) {
    int i,j,k,n=5;
    for(i=1;i<=n;i++){
        for(j=1;j<=i;j++){
            printf("%d ",j);
        }
        for(j=i-1;j>0;j--){
            printf("%d ",j);
        }
        printf("\n");
    }
}
```

</details>

---

## Pattern 26 <p align="right"> [🔝 Back to Index](#index) </p>

```c
1 * * * * * * 1 
1 2 * * * * 2 1 
1 2 3 * * 3 2 1 
1 2 3 4 4 3 2 1 
```
<details>
<summary> 👉 Click to view the Code of Pattern 26 </summary>

```c
#include <stdio.h>

int main(void) {
    int i,j,n=4;
    for(i=1;i<=n;i++){
        for(j=1;j<=i;j++){
            printf("%d ",j);
        }
        for(j=(n-i)*2;j>=1;j--){
            printf("* ");
        }
        for(j=i;j>0;j--){
            printf("%d ",j);
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 27 <p align="right"> [🔝 Back to Index](#index) </p>

```c
1 2 3 4 4 3 2 1 
1 2 3 * * 3 2 1 
1 2 * * * * 2 1 
1 * * * * * * 1 
```
<details>
<summary> 👉 Click to view the Code of Pattern 27 </summary>

```c
#include <stdio.h>

int main(void) {
    int i,j,n=4;
    for(i=0;i<n;i++){
        for(j=1;j<=n-i;j++){
            printf("%d ",j);
        }
        for(j=0;j<2*i;j++){
            printf("* ");
        }
        for(j=n-i;j>0;j--){
            printf("%d ",j);
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 28 <p align="right"> [🔝 Back to Index](#index) </p>

```c
1 3 5 7 9 
3 5 7 9 
5 7 9 
7 9 
9 
```
<details>
<summary> 👉 Click to view the Code of Pattern 28 </summary>

```c
#include <stdio.h>

int main(void) {
    int i,j,k,n=5;
    for(i=1;i<=2*n;i+=2){
        for(j=i;j<2*n;j+=2){
            printf("%d ",j);
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 29 <p align="right"> [🔝 Back to Index](#index) </p>

```c
* * * * * * * * * * * * * 
* * 
* * * * * * * * * * * 
* * 
* * * * * * * * * 
* * 
* * * * * * * 
* * 
* * * * * 
* * 
* * * 
* * 
* 
```
<details>
<summary> 👉 Click to view the Code of Pattern 29 </summary>

```c
#include <stdio.h>

int main(void) {
int i,j,n=7;
    for(i=0;i<n;i++){
        for(j=0;j<(n-i)*2-1;j++){
            printf("* ");
        }
        printf("\n");
        if(i==n-1){
            break;
        }
        for(j=0;j<2;j++){
            printf("* ");
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 30 <p align="right"> [🔝 Back to Index](#index) </p>

```c
*
* 
* * * 
* * 
* * 
* * * * * * 
* * * 
* * * 
* * * 
* * * * * * * * * 
```
<details>
<summary> 👉 Click to view the Code of Pattern 30 </summary>

```c
#include <stdio.h>

int main(void) {
    int i,j,k,n=4;
    for(i=1;i<n;i++){
        if(i==1){
            printf("*\n");
        }
        for(k=0;k<i;k++){
            for(j=0;j<i;j++){
                printf("* ");
            }
            printf("\n");
        }
        for(k=1;k<=3*i;k++){
            printf("* ");
        }
        printf("\n");
    }
}
```
</details>

---

## Pattern 31 <p align="right"> [🔝 Back to Index](#index) </p>


```c

0 1 
0 2 4 
0 3 6 9 
0 4 8 12 16 
0 5 10 15 20 25 
0 6 12 18 24 30 36 
```

<details>

<summary> 👉 Click to view the Code of Pattern 31 </summary>


```c

#include <stdio.h>

int main(void) {
    int i,j,n=6;
    for(i=1;i<=n;i++){
        for(j=0;j<=i;j++){
            printf("%d ",i*j);
        }
        printf("\n");
    }
}
```

</details>

---






[//]: # ()
[//]: # (## Pattern )

[//]: # ()
[//]: # (```c)

[//]: # ()
[//]: # (```)

[//]: # (<details>)

[//]: # (<summary> 👉 Click to view the Code of Pattern  </summary>)

[//]: # ()
[//]: # (```c)

[//]: # ()
[//]: # (```)

[//]: # (</details>)

