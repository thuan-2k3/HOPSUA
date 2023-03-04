# HOPSUA


#include<stdio.h>
#include<conio.h>

struct HOPSUA
{
    int ngay ;
    float trongluong ;
    char nhanhieu [20] ;
};
 typedef struct  HOPSUA hs ;

 void nhapthongtin ( hs  hs  )
 {
    printf("nhap vao nhan hieu : ");
    scanf("%s", &hs.nhanhieu );

    printf(" nhap vao trong luong ");
    scanf("%2f", hs.trongluong );

    printf(" nhap vao ngay su dung : ");
    scanf("%d", hs.ngay );
 };
 
 void xuatthongtin (hs hs )
 {
    printf("nhan hieu : %s \n", hs.nhanhieu );
    printf("truong luong : %2f \n", hs.trongluong );
    printf("han su dung : %d \n", hs.ngay );
 
 }

 int main()
 {
    HOPSUA hs ;
    nhapthongtin(hs);
    xuatthongtin(hs);
    getch ;
    return 0;
    
 }
