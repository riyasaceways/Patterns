# Patterns
Patterns with code

## Pattern 1

```c
0|0  0|1  0|2  0|3  0|4

1|0  1|1  1|2  1|3  1|4

2|0  2|1  2|2  2|3  2|4

3|0  3|1  3|2  3|3  3|4

4|0  4|1  4|2  4|3  4|4
```
<p>This Grid pattern to understand the cound of grid of </p>

<details>

<summary> 👆Click to view the Code of Pattern 1 </summary>

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
## Pattern 2
```c
50 
45 40 
35 30 25 
20 15 10 5 
```

<details>
<summary> 👆Click to view the Code of Pattern 2 </summary>

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

## Pattern 3
```c
*       * 
* *     * 
*   *   * 
*     * * 
*       * 
```
<details>
<summary> 👆Click to view the Code of Pattern 3 </summary>

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

## Pattern 4

```c
* * * * * 
      *   
    *     
  *       
* * * * * 
```
<details>
<summary> 👆Click to view the Code of Pattern 4 </summary>

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

## Pattern 5

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
<summary> 👆Click to view the Code of Pattern 5 </summary>

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

## Pattern 6

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
<summary> 👆Click to view the Code of Pattern 6 </summary>

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

## Pattern 7

```c
      *
     * *
    *   *
   *     *
  *       *
 ***********
```
<details>
<summary> 👆Click to view the Code of Pattern 7 </summary>
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
## Pattern 8

```c
1 
1 2 
1   3 
1     4 
1 2 3 4 5 
```
<details>
<summary> 👆Click to view the Code of Pattern 8 </summary>

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
## Pattern 9

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
<summary> 👆Click to view the Code of Pattern 9 </summary>

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
<summary> 👆Click to view the Code of Pattern 10 </summary>

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


## Pattern 11

```c
*                         * 
                          
* * *                 * * * 
                        
* * * * *         * * * * * 
                      
* * * * * * * * * * * * * * 
```
<details>
<summary> 👆Click to view the Code of Pattern 11 </summary>

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


## Pattern 12

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
<summary> 👆Click to view the Code of Pattern 12 </summary>

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

## Pattern 13

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
<summary> 👆Click to view the Code of Pattern 13</summary>

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

[//]: # ()
[//]: # (## Pattern )

[//]: # ()
[//]: # (```c)

[//]: # ()
[//]: # (```)

[//]: # (<details>)

[//]: # (<summary> 👆Click to view the Code of Pattern  </summary>)

[//]: # ()
[//]: # (```c)

[//]: # ()
[//]: # (```)

[//]: # (</details>)


---