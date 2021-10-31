# sansli cekilis uygulamasi











#include <stdio.h>
#include <stdlib.h>
#include <time.h>
#include<conio.h>
int main(){
	printf("MADE BY: FURBLOOD13 (github username)  \n\n");
	
    char isim[10];
	char soyisim[10];
	int secim;
	int sayi;
	printf("LUTFEN ISMINIZI GIRINIZ:");
	scanf("%s" , &isim);
	printf("\nLUTFEN SOYISMINIZI GIRINIZ:");
	scanf ("%s", &soyisim);
	printf("\n asagidaki islemlerden birini seciniz:");
	printf(" \n [1]-sansli cekilisi dene \n [2]-kullanici bilgilerini kontrol et \n \n SECIMINIZ:");
	scanf("%d" , &secim);
	if(secim==1){
		printf("\n BIR ILE BES ARASINDAN BIR SAYI SECINIZ: ");
		scanf("%d" , &sayi);
		srand(time(NULL));
		int random=1+rand()%5;
		if(sayi==random){
			printf("\n \n GIRDIGINIZ SAYI: %d " , sayi);
			
			printf("\n \n CEKILISTEKI SAYI: %d" , random);
			
				
			printf("\n \n \t TEBRIKLER DOGRU BILDIN");
			
		}
		else {
		printf("\n GIRDIGINIZ SAYI: %d \n \n CEKILISTEKI SAYI: %d" , sayi , random);
		printf ("\n \n \t UZGUNUZ SANSINIZI BIRDAHA DENEYINIZ");
		
		}
		
		
		
	}	
	
	else if(secim==2){
		printf("kullanici adiniz: %s \n kullanici soyadiniz: %s" , isim , soyisim);
		
	}
		getch();
		
		return 0;
		
	}

