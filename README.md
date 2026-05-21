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
<p>This Grid pattern to understand the cound of p</p>

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





## Pattern 6

```c
      *
     * *
    *   *
   *     *
  *       *
 ***********
```
<details>
<summary> 👆Click to view the Code of Pattern 6 </summary>

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