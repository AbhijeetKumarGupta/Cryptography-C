#include <stdlib.h>
#include <stdio.h>
#include <string.h>
#include <conio.h>

int main() {

	int Opt, Con, Key;

	do{

		system("cls");
		printf("    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~");
		printf("\n    WELCOME TO THE ENCRYPTION AND DECRYPTION TERMINAL");
		printf("\n    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~");
		printf("\n**************************");
		printf("\nWhat would you like to do?");
		printf("\n**************************");
		printf("\n");
		printf("[1] ENCRYPTION.\n");
		printf("[2] DECRYPTION.\n");
		printf("[3] QUIT.");
		printf("\n\n");
		scanf("%d",&Opt);
		system("cls");

		if(Opt == 1){

			printf("\nSelect Encryption Key:-\n");
			printf("[1] KEY 1.\n");
			printf("[2] KEY 2.\n");
			printf("[3] KEY 3.\n");
			printf("[4] KEY 4.\n");
			scanf("%d",&Key);

			if(Key == 1){

				system("cls");

				char Key_Reg[65] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m',
									'n','o','p','q','r','s','t','u','v','w','x','y','z',' ','1','2','3','4','5','6','7','8','9','0','.'};

				char Key_Enc[129] = {'~','-','/','{','`','=','?','+','!','q','.','l','@','r','>','k','#','s',',','n','$','t','<','i','%','u','"','h','^','v',';','g','&','w','f',':','x','*','c',
									'|','y','(','b',']','z',')','d','}','a','_','e','[','-','~','{','/','=','`','+','?','q','!','l','.','r','@','k','>','s','#','n',',','t','$','i','<','u','%',
									'h','"','v','^','g',';','w','&',':','f','*','x','|','c','(','y',']','b',')','z','}','d','_','a','[','e','$','$','9','!','!','8','7','!','!','6','5','!','!',
									'4','3','!','!','2','1','!','!','!','{','}'};


				int Strlen_Enc = 0, Strlen_Reg = 0, n=0, k=0;
				char v;
				char Ept[8000];
				char Str_Reg[4000];
				char Str_Enc[8000];

				printf("    ~~~~~~~~~~~~~~~~~~~");
				printf("\n    ENCRYPTION TERMINAL");
				printf("\n    ~~~~~~~~~~~~~~~~~~~");
				printf("\n******************************************");
				printf("\nEnter the text you want to encrypt below:-");
				printf("\n******************************************");
				printf("\n");
				printf("---------");
				printf("\n-REGULAR-");
				printf("\n---------");
				printf("\n\n");

				scanf("%c",&v);
				gets(Str_Reg);

				Strlen_Reg = strlen(Str_Reg);


				while(n != Strlen_Reg){

									if(Str_Reg[n] == Key_Reg[0]){

										Str_Enc[k] = Key_Enc[0];
										Str_Enc[k+1] = Key_Enc[1];

									}else if(Str_Reg[n] == Key_Reg[1]){

										Str_Enc[k] = Key_Enc[2];
										Str_Enc[k+1] = Key_Enc[3];

									}else if(Str_Reg[n] == Key_Reg[2]){

										Str_Enc[k] = Key_Enc[4];
										Str_Enc[k+1] = Key_Enc[5];

									}else if(Str_Reg[n] == Key_Reg[3]){

										Str_Enc[k] = Key_Enc[6];
										Str_Enc[k+1] = Key_Enc[7];

									}else if(Str_Reg[n] == Key_Reg[4]){

										Str_Enc[k] = Key_Enc[8];
										Str_Enc[k+1] = Key_Enc[9];

									}else if(Str_Reg[n] == Key_Reg[5]){

										Str_Enc[k] = Key_Enc[10];
										Str_Enc[k+1] = Key_Enc[11];

									}else if(Str_Reg[n] == Key_Reg[6]){

										Str_Enc[k] = Key_Enc[12];
										Str_Enc[k+1] = Key_Enc[13];

									}else if(Str_Reg[n] == Key_Reg[7]){

										Str_Enc[k] = Key_Enc[14];
										Str_Enc[k+1] = Key_Enc[15];

									}else if(Str_Reg[n] == Key_Reg[8]){

										Str_Enc[k] = Key_Enc[16];
										Str_Enc[k+1] = Key_Enc[17];

									}else if(Str_Reg[n] == Key_Reg[9]){

										Str_Enc[k] = Key_Enc[18];
										Str_Enc[k+1] = Key_Enc[19];

									}else if(Str_Reg[n] == Key_Reg[10]){

										Str_Enc[k] = Key_Enc[20];
										Str_Enc[k+1] = Key_Enc[21];

									}else if(Str_Reg[n] == Key_Reg[11]){

										Str_Enc[k] = Key_Enc[22];
										Str_Enc[k+1] = Key_Enc[23];

									}else if(Str_Reg[n] == Key_Reg[12]){

										Str_Enc[k] = Key_Enc[24];
										Str_Enc[k+1] = Key_Enc[25];

									}else if(Str_Reg[n] == Key_Reg[13]){

										Str_Enc[k] = Key_Enc[26];
										Str_Enc[k+1] = Key_Enc[27];

									}else if(Str_Reg[n] == Key_Reg[14]){

										Str_Enc[k] = Key_Enc[28];
										Str_Enc[k+1] = Key_Enc[29];

									}else if(Str_Reg[n] == Key_Reg[15]){

										Str_Enc[k] = Key_Enc[30];
										Str_Enc[k+1] = Key_Enc[31];

									}else if(Str_Reg[n] == Key_Reg[16]){

										Str_Enc[k] = Key_Enc[32];
										Str_Enc[k+1] = Key_Enc[33];

									}else if(Str_Reg[n] == Key_Reg[17]){

										Str_Enc[k] = Key_Enc[34];
										Str_Enc[k+1] = Key_Enc[35];

									}else if(Str_Reg[n] == Key_Reg[18]){

										Str_Enc[k] = Key_Enc[36];
										Str_Enc[k+1] = Key_Enc[37];

									}else if(Str_Reg[n] == Key_Reg[19]){

										Str_Enc[k] = Key_Enc[38];
										Str_Enc[k+1] = Key_Enc[39];

									}else if(Str_Reg[n] == Key_Reg[20]){

										Str_Enc[k] = Key_Enc[40];
										Str_Enc[k+1] = Key_Enc[41];

									}else if(Str_Reg[n] == Key_Reg[21]){

										Str_Enc[k] = Key_Enc[42];
										Str_Enc[k+1] = Key_Enc[43];

									}else if(Str_Reg[n] == Key_Reg[22]){

										Str_Enc[k] = Key_Enc[44];
										Str_Enc[k+1] = Key_Enc[45];

									}else if(Str_Reg[n] == Key_Reg[23]){

										Str_Enc[k] = Key_Enc[46];
										Str_Enc[k+1] = Key_Enc[47];

									}else if(Str_Reg[n] == Key_Reg[24]){

										Str_Enc[k] = Key_Enc[48];
										Str_Enc[k+1] = Key_Enc[49];

									}else if(Str_Reg[n] == Key_Reg[25]){

										Str_Enc[k] = Key_Enc[50];
										Str_Enc[k+1] = Key_Enc[51];

									}else if(Str_Reg[n] == Key_Reg[26]){

										Str_Enc[k] = Key_Enc[52];
										Str_Enc[k+1] = Key_Enc[53];

									}else if(Str_Reg[n] == Key_Reg[27]){

										Str_Enc[k] = Key_Enc[54];
										Str_Enc[k+1] = Key_Enc[55];

									}else if(Str_Reg[n] == Key_Reg[28]){

										Str_Enc[k] = Key_Enc[56];
										Str_Enc[k+1] = Key_Enc[57];

									}else if(Str_Reg[n] == Key_Reg[29]){

										Str_Enc[k] = Key_Enc[58];
										Str_Enc[k+1] = Key_Enc[59];

									}else if(Str_Reg[n] == Key_Reg[30]){

										Str_Enc[k] = Key_Enc[60];
										Str_Enc[k+1] = Key_Enc[61];

									}else if(Str_Reg[n] == Key_Reg[31]){

										Str_Enc[k] = Key_Enc[62];
										Str_Enc[k+1] = Key_Enc[63];

									}else if(Str_Reg[n] == Key_Reg[32]){

										Str_Enc[k] = Key_Enc[64];
										Str_Enc[k+1] = Key_Enc[65];

									}else if(Str_Reg[n] == Key_Reg[33]){

										Str_Enc[k] = Key_Enc[66];
										Str_Enc[k+1] = Key_Enc[67];

									}else if(Str_Reg[n] == Key_Reg[34]){

										Str_Enc[k] = Key_Enc[68];
										Str_Enc[k+1] = Key_Enc[69];

									}else if(Str_Reg[n] == Key_Reg[35]){

										Str_Enc[k] = Key_Enc[70];
										Str_Enc[k+1] = Key_Enc[71];

									}else if(Str_Reg[n] == Key_Reg[36]){

										Str_Enc[k] = Key_Enc[72];
										Str_Enc[k+1] = Key_Enc[73];

									}else if(Str_Reg[n] == Key_Reg[37]){

										Str_Enc[k] = Key_Enc[74];
										Str_Enc[k+1] = Key_Enc[75];

									}else if(Str_Reg[n] == Key_Reg[38]){

										Str_Enc[k] = Key_Enc[76];
										Str_Enc[k+1] = Key_Enc[77];

									}else if(Str_Reg[n] == Key_Reg[39]){

										Str_Enc[k] = Key_Enc[78];
										Str_Enc[k+1] = Key_Enc[79];

									}else if(Str_Reg[n] == Key_Reg[40]){

										Str_Enc[k] = Key_Enc[80];
										Str_Enc[k+1] = Key_Enc[81];

									}else if(Str_Reg[n] == Key_Reg[41]){

										Str_Enc[k] = Key_Enc[82];
										Str_Enc[k+1] = Key_Enc[83];

									}else if(Str_Reg[n] == Key_Reg[42]){

										Str_Enc[k] = Key_Enc[84];
										Str_Enc[k+1] = Key_Enc[85];

									}else if(Str_Reg[n] == Key_Reg[43]){

										Str_Enc[k] = Key_Enc[86];
										Str_Enc[k+1] = Key_Enc[87];

									}else if(Str_Reg[n] == Key_Reg[44]){

										Str_Enc[k] = Key_Enc[88];
										Str_Enc[k+1] = Key_Enc[89];

									}else if(Str_Reg[n] == Key_Reg[45]){

										Str_Enc[k] = Key_Enc[90];
										Str_Enc[k+1] = Key_Enc[91];

									}else if(Str_Reg[n] == Key_Reg[46]){

										Str_Enc[k] = Key_Enc[92];
										Str_Enc[k+1] = Key_Enc[93];

									}else if(Str_Reg[n] == Key_Reg[47]){

										Str_Enc[k] = Key_Enc[94];
										Str_Enc[k+1] = Key_Enc[95];

									}else if(Str_Reg[n] == Key_Reg[48]){

										Str_Enc[k] = Key_Enc[96];
										Str_Enc[k+1] = Key_Enc[97];

									}else if(Str_Reg[n] == Key_Reg[49]){

										Str_Enc[k] = Key_Enc[98];
										Str_Enc[k+1] = Key_Enc[99];

									}else if(Str_Reg[n] == Key_Reg[50]){

										Str_Enc[k] = Key_Enc[100];
										Str_Enc[k+1] = Key_Enc[101];

									}else if(Str_Reg[n] == Key_Reg[51]){

										Str_Enc[k] = Key_Enc[102];
										Str_Enc[k+1] = Key_Enc[103];

									}else if(Str_Reg[n] == Key_Reg[52]){

										Str_Enc[k] = Key_Enc[104];
										Str_Enc[k+1] = Key_Enc[105];

									}else if(Str_Reg[n] == Key_Reg[53]){

										Str_Enc[k] = Key_Enc[106];
										Str_Enc[k+1] = Key_Enc[107];

									}else if(Str_Reg[n] == Key_Reg[54]){

										Str_Enc[k] = Key_Enc[108];
										Str_Enc[k+1] = Key_Enc[109];

									}else if(Str_Reg[n] == Key_Reg[55]){

										Str_Enc[k] = Key_Enc[110];
										Str_Enc[k+1] = Key_Enc[111];

									}else if(Str_Reg[n] == Key_Reg[56]){

										Str_Enc[k] = Key_Enc[112];
										Str_Enc[k+1] = Key_Enc[113];

									}else if(Str_Reg[n] == Key_Reg[57]){

										Str_Enc[k] = Key_Enc[114];
										Str_Enc[k+1] = Key_Enc[115];

									}else if(Str_Reg[n] == Key_Reg[58]){

										Str_Enc[k] = Key_Enc[116];
										Str_Enc[k+1] = Key_Enc[117];

									}else if(Str_Reg[n] == Key_Reg[59]){

										Str_Enc[k] = Key_Enc[118];
										Str_Enc[k+1] = Key_Enc[119];

									}else if(Str_Reg[n] == Key_Reg[60]){

										Str_Enc[k] = Key_Enc[120];
										Str_Enc[k+1] = Key_Enc[121];

									}else if(Str_Reg[n] == Key_Reg[61]){

										Str_Enc[k] = Key_Enc[122];
										Str_Enc[k+1] = Key_Enc[123];

									}else if(Str_Reg[n] == Key_Reg[62]){

										Str_Enc[k] = Key_Enc[124];
										Str_Enc[k+1] = Key_Enc[125];

									}else if(Str_Reg[n] == Key_Reg[63]){

										Str_Enc[k] = Key_Enc[126];
										Str_Enc[k+1] = Key_Enc[127];

									}

									n = n+1;
									k = k+2;

								}

								printf("\n");
								printf("-----------");
								printf("\n-ENCRYPTED-");
								printf("\n-----------");
								printf("\n\n");

								Strlen_Enc = strlen(Str_Enc);

								for(k=0;k<Strlen_Enc;k++){

									printf("%c",Str_Enc[k]);
									Str_Enc[k]=Ept[k];
									Str_Reg[k]=Ept[k];
								}


								scanf("%c",&v);

			}else if(Key == 2){

				system("cls");
				char Key_Reg[65] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m',
													'n','o','p','q','r','s','t','u','v','w','x','y','z',' ','1','2','3','4','5','6','7','8','9','0','.'};

				char Key_Enc[129] = {'e','[','a','_','d','}','z',')','b',']','y','(','c','|','x','*','f',':','&','w',';','g','^','v','"','h','%','u','<','i','$','t',',','n','#','s','>','k','@',
										'r','.','l','!','q','?','+','`','=','/','{','~','-','[','e','_','a','}','d',')','z',']','b','(','y','|','c','*','x',':','f','w','&','g',';','v','^','h','"',
										'u','%','i','<','t','$','n',',','s','#','k','>','r','@','l','.','q','!','+','?','=','`','{','/','-','~','$','$','9','!','!','8','7','!','!','6','5','!','!',
										'4','3','!','!','2','1','!','!','!','{','}'};

				int Strlen_Enc = 0, Strlen_Reg = 0, n=0, k=0;
				char v;
				char Ept[8000];
			    char Str_Reg[4000];
				char Str_Enc[8000];

				printf("    ~~~~~~~~~~~~~~~~~~~");
			    printf("\n    ENCRYPTION TERMINAL");
			    printf("\n    ~~~~~~~~~~~~~~~~~~~");
				printf("\n******************************************");
				printf("\nEnter the text you want to encrypt below:-");
				printf("\n******************************************");
				printf("\n");
				printf("---------");
				printf("\n-REGULAR-");
				printf("\n---------");
				printf("\n\n");

				scanf("%c",&v);
				gets(Str_Reg);

				Strlen_Reg = strlen(Str_Reg);

				while(n != Strlen_Reg){

									if(Str_Reg[n] == Key_Reg[0]){

										Str_Enc[k] = Key_Enc[0];
										Str_Enc[k+1] = Key_Enc[1];

									}else if(Str_Reg[n] == Key_Reg[1]){

										Str_Enc[k] = Key_Enc[2];
										Str_Enc[k+1] = Key_Enc[3];

									}else if(Str_Reg[n] == Key_Reg[2]){

										Str_Enc[k] = Key_Enc[4];
										Str_Enc[k+1] = Key_Enc[5];

									}else if(Str_Reg[n] == Key_Reg[3]){

										Str_Enc[k] = Key_Enc[6];
										Str_Enc[k+1] = Key_Enc[7];

									}else if(Str_Reg[n] == Key_Reg[4]){

										Str_Enc[k] = Key_Enc[8];
										Str_Enc[k+1] = Key_Enc[9];

									}else if(Str_Reg[n] == Key_Reg[5]){

										Str_Enc[k] = Key_Enc[10];
										Str_Enc[k+1] = Key_Enc[11];

									}else if(Str_Reg[n] == Key_Reg[6]){

										Str_Enc[k] = Key_Enc[12];
										Str_Enc[k+1] = Key_Enc[13];

									}else if(Str_Reg[n] == Key_Reg[7]){

										Str_Enc[k] = Key_Enc[14];
										Str_Enc[k+1] = Key_Enc[15];

									}else if(Str_Reg[n] == Key_Reg[8]){

										Str_Enc[k] = Key_Enc[16];
										Str_Enc[k+1] = Key_Enc[17];

									}else if(Str_Reg[n] == Key_Reg[9]){

										Str_Enc[k] = Key_Enc[18];
										Str_Enc[k+1] = Key_Enc[19];

									}else if(Str_Reg[n] == Key_Reg[10]){

										Str_Enc[k] = Key_Enc[20];
										Str_Enc[k+1] = Key_Enc[21];

									}else if(Str_Reg[n] == Key_Reg[11]){

										Str_Enc[k] = Key_Enc[22];
										Str_Enc[k+1] = Key_Enc[23];

									}else if(Str_Reg[n] == Key_Reg[12]){

										Str_Enc[k] = Key_Enc[24];
										Str_Enc[k+1] = Key_Enc[25];

									}else if(Str_Reg[n] == Key_Reg[13]){

										Str_Enc[k] = Key_Enc[26];
										Str_Enc[k+1] = Key_Enc[27];

									}else if(Str_Reg[n] == Key_Reg[14]){

										Str_Enc[k] = Key_Enc[28];
										Str_Enc[k+1] = Key_Enc[29];

									}else if(Str_Reg[n] == Key_Reg[15]){

										Str_Enc[k] = Key_Enc[30];
										Str_Enc[k+1] = Key_Enc[31];

									}else if(Str_Reg[n] == Key_Reg[16]){

										Str_Enc[k] = Key_Enc[32];
										Str_Enc[k+1] = Key_Enc[33];

									}else if(Str_Reg[n] == Key_Reg[17]){

										Str_Enc[k] = Key_Enc[34];
										Str_Enc[k+1] = Key_Enc[35];

									}else if(Str_Reg[n] == Key_Reg[18]){

										Str_Enc[k] = Key_Enc[36];
										Str_Enc[k+1] = Key_Enc[37];

									}else if(Str_Reg[n] == Key_Reg[19]){

										Str_Enc[k] = Key_Enc[38];
										Str_Enc[k+1] = Key_Enc[39];

									}else if(Str_Reg[n] == Key_Reg[20]){

										Str_Enc[k] = Key_Enc[40];
										Str_Enc[k+1] = Key_Enc[41];

									}else if(Str_Reg[n] == Key_Reg[21]){

										Str_Enc[k] = Key_Enc[42];
										Str_Enc[k+1] = Key_Enc[43];

									}else if(Str_Reg[n] == Key_Reg[22]){

										Str_Enc[k] = Key_Enc[44];
										Str_Enc[k+1] = Key_Enc[45];

									}else if(Str_Reg[n] == Key_Reg[23]){

										Str_Enc[k] = Key_Enc[46];
										Str_Enc[k+1] = Key_Enc[47];

									}else if(Str_Reg[n] == Key_Reg[24]){

										Str_Enc[k] = Key_Enc[48];
										Str_Enc[k+1] = Key_Enc[49];

									}else if(Str_Reg[n] == Key_Reg[25]){

										Str_Enc[k] = Key_Enc[50];
										Str_Enc[k+1] = Key_Enc[51];

									}else if(Str_Reg[n] == Key_Reg[26]){

										Str_Enc[k] = Key_Enc[52];
										Str_Enc[k+1] = Key_Enc[53];

									}else if(Str_Reg[n] == Key_Reg[27]){

										Str_Enc[k] = Key_Enc[54];
										Str_Enc[k+1] = Key_Enc[55];

									}else if(Str_Reg[n] == Key_Reg[28]){

										Str_Enc[k] = Key_Enc[56];
										Str_Enc[k+1] = Key_Enc[57];

									}else if(Str_Reg[n] == Key_Reg[29]){

										Str_Enc[k] = Key_Enc[58];
										Str_Enc[k+1] = Key_Enc[59];

									}else if(Str_Reg[n] == Key_Reg[30]){

										Str_Enc[k] = Key_Enc[60];
										Str_Enc[k+1] = Key_Enc[61];

									}else if(Str_Reg[n] == Key_Reg[31]){

										Str_Enc[k] = Key_Enc[62];
										Str_Enc[k+1] = Key_Enc[63];

									}else if(Str_Reg[n] == Key_Reg[32]){

										Str_Enc[k] = Key_Enc[64];
										Str_Enc[k+1] = Key_Enc[65];

									}else if(Str_Reg[n] == Key_Reg[33]){

										Str_Enc[k] = Key_Enc[66];
										Str_Enc[k+1] = Key_Enc[67];

									}else if(Str_Reg[n] == Key_Reg[34]){

										Str_Enc[k] = Key_Enc[68];
										Str_Enc[k+1] = Key_Enc[69];

									}else if(Str_Reg[n] == Key_Reg[35]){

										Str_Enc[k] = Key_Enc[70];
										Str_Enc[k+1] = Key_Enc[71];

									}else if(Str_Reg[n] == Key_Reg[36]){

										Str_Enc[k] = Key_Enc[72];
										Str_Enc[k+1] = Key_Enc[73];

									}else if(Str_Reg[n] == Key_Reg[37]){

										Str_Enc[k] = Key_Enc[74];
										Str_Enc[k+1] = Key_Enc[75];

									}else if(Str_Reg[n] == Key_Reg[38]){

										Str_Enc[k] = Key_Enc[76];
										Str_Enc[k+1] = Key_Enc[77];

									}else if(Str_Reg[n] == Key_Reg[39]){

										Str_Enc[k] = Key_Enc[78];
										Str_Enc[k+1] = Key_Enc[79];

									}else if(Str_Reg[n] == Key_Reg[40]){

										Str_Enc[k] = Key_Enc[80];
										Str_Enc[k+1] = Key_Enc[81];

									}else if(Str_Reg[n] == Key_Reg[41]){

										Str_Enc[k] = Key_Enc[82];
										Str_Enc[k+1] = Key_Enc[83];

									}else if(Str_Reg[n] == Key_Reg[42]){

										Str_Enc[k] = Key_Enc[84];
										Str_Enc[k+1] = Key_Enc[85];

									}else if(Str_Reg[n] == Key_Reg[43]){

										Str_Enc[k] = Key_Enc[86];
										Str_Enc[k+1] = Key_Enc[87];

									}else if(Str_Reg[n] == Key_Reg[44]){

										Str_Enc[k] = Key_Enc[88];
										Str_Enc[k+1] = Key_Enc[89];

									}else if(Str_Reg[n] == Key_Reg[45]){

										Str_Enc[k] = Key_Enc[90];
										Str_Enc[k+1] = Key_Enc[91];

									}else if(Str_Reg[n] == Key_Reg[46]){

										Str_Enc[k] = Key_Enc[92];
										Str_Enc[k+1] = Key_Enc[93];

									}else if(Str_Reg[n] == Key_Reg[47]){

										Str_Enc[k] = Key_Enc[94];
										Str_Enc[k+1] = Key_Enc[95];

									}else if(Str_Reg[n] == Key_Reg[48]){

										Str_Enc[k] = Key_Enc[96];
										Str_Enc[k+1] = Key_Enc[97];

									}else if(Str_Reg[n] == Key_Reg[49]){

										Str_Enc[k] = Key_Enc[98];
										Str_Enc[k+1] = Key_Enc[99];

									}else if(Str_Reg[n] == Key_Reg[50]){

										Str_Enc[k] = Key_Enc[100];
										Str_Enc[k+1] = Key_Enc[101];

									}else if(Str_Reg[n] == Key_Reg[51]){

										Str_Enc[k] = Key_Enc[102];
										Str_Enc[k+1] = Key_Enc[103];

									}else if(Str_Reg[n] == Key_Reg[52]){

										Str_Enc[k] = Key_Enc[104];
										Str_Enc[k+1] = Key_Enc[105];

									}else if(Str_Reg[n] == Key_Reg[53]){

										Str_Enc[k] = Key_Enc[106];
										Str_Enc[k+1] = Key_Enc[107];

									}else if(Str_Reg[n] == Key_Reg[54]){

										Str_Enc[k] = Key_Enc[108];
										Str_Enc[k+1] = Key_Enc[109];

									}else if(Str_Reg[n] == Key_Reg[55]){

										Str_Enc[k] = Key_Enc[110];
										Str_Enc[k+1] = Key_Enc[111];

									}else if(Str_Reg[n] == Key_Reg[56]){

										Str_Enc[k] = Key_Enc[112];
										Str_Enc[k+1] = Key_Enc[113];

									}else if(Str_Reg[n] == Key_Reg[57]){

										Str_Enc[k] = Key_Enc[114];
										Str_Enc[k+1] = Key_Enc[115];

									}else if(Str_Reg[n] == Key_Reg[58]){

										Str_Enc[k] = Key_Enc[116];
										Str_Enc[k+1] = Key_Enc[117];

									}else if(Str_Reg[n] == Key_Reg[59]){

										Str_Enc[k] = Key_Enc[118];
										Str_Enc[k+1] = Key_Enc[119];

									}else if(Str_Reg[n] == Key_Reg[60]){

										Str_Enc[k] = Key_Enc[120];
										Str_Enc[k+1] = Key_Enc[121];

									}else if(Str_Reg[n] == Key_Reg[61]){

										Str_Enc[k] = Key_Enc[122];
										Str_Enc[k+1] = Key_Enc[123];

									}else if(Str_Reg[n] == Key_Reg[62]){

										Str_Enc[k] = Key_Enc[124];
										Str_Enc[k+1] = Key_Enc[125];

									}else if(Str_Reg[n] == Key_Reg[63]){

										Str_Enc[k] = Key_Enc[126];
										Str_Enc[k+1] = Key_Enc[127];

									}

									n = n+1;
									k = k+2;

								}

								printf("\n");
								printf("-----------");
								printf("\n-ENCRYPTED-");
								printf("\n-----------");
								printf("\n\n");

								Strlen_Enc = strlen(Str_Enc);

								for(k=0;k<Strlen_Enc;k++){
									printf("%c",Str_Enc[k]);
									Str_Enc[k]=Ept[k];
									Str_Reg[k]=Ept[k];
								}

								scanf("%c",&v);

			}else if(Key == 3){

				system("cls");

				char Key_Reg[65] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m',
													'n','o','p','q','r','s','t','u','v','w','x','y','z',' ','1','2','3','4','5','6','7','8','9','0','.'};

				char Key_Enc[129] = {'"','h','^','v',';','g','&','w','f',':','x','*','c','|','y','(','b',']','z',')','d','}','a','_','e','[','~','-','/','{','`','=','?','+','!','q','.','l','@',
										'r','>','k','#','s',',','n','$','t','<','i','%','u','h','"','v','^','g',';','w','&',':','f','*','x','|','c','(','y',']','b',')','z','}','d','_','a','[','e',
										'-','~','{','/','=','`','+','?','q','!','l','.','r','@','k','>','s','#','n',',','t','$','i','<','u','%','$','$','9','!','!','8','7','!','!','6','5','!','!',
										'4','3','!','!','2','1','!','!','!','{','}'};

								int Strlen_Enc = 0, Strlen_Reg = 0, n=0, k=0;
								char v;
								char Ept[8000];
								char Str_Reg[4000];
								char Str_Enc[8000];

								printf("    ~~~~~~~~~~~~~~~~~~~");
								printf("\n    ENCRYPTION TERMINAL");
								printf("\n    ~~~~~~~~~~~~~~~~~~~");
								printf("\n******************************************");
								printf("\nEnter the text you want to encrypt below:-");
								printf("\n******************************************");
								printf("\n");
								printf("---------");
								printf("\n-REGULAR-");
								printf("\n---------");
								printf("\n\n");

								scanf("%c",&v);
								gets(Str_Reg);

								Strlen_Reg = strlen(Str_Reg);

								while(n != Strlen_Reg){

									if(Str_Reg[n] == Key_Reg[0]){

										Str_Enc[k] = Key_Enc[0];
										Str_Enc[k+1] = Key_Enc[1];

									}else if(Str_Reg[n] == Key_Reg[1]){

										Str_Enc[k] = Key_Enc[2];
										Str_Enc[k+1] = Key_Enc[3];

									}else if(Str_Reg[n] == Key_Reg[2]){

										Str_Enc[k] = Key_Enc[4];
										Str_Enc[k+1] = Key_Enc[5];

									}else if(Str_Reg[n] == Key_Reg[3]){

										Str_Enc[k] = Key_Enc[6];
										Str_Enc[k+1] = Key_Enc[7];

									}else if(Str_Reg[n] == Key_Reg[4]){

										Str_Enc[k] = Key_Enc[8];
										Str_Enc[k+1] = Key_Enc[9];

									}else if(Str_Reg[n] == Key_Reg[5]){

										Str_Enc[k] = Key_Enc[10];
										Str_Enc[k+1] = Key_Enc[11];

									}else if(Str_Reg[n] == Key_Reg[6]){

										Str_Enc[k] = Key_Enc[12];
										Str_Enc[k+1] = Key_Enc[13];

									}else if(Str_Reg[n] == Key_Reg[7]){

										Str_Enc[k] = Key_Enc[14];
										Str_Enc[k+1] = Key_Enc[15];

									}else if(Str_Reg[n] == Key_Reg[8]){

										Str_Enc[k] = Key_Enc[16];
										Str_Enc[k+1] = Key_Enc[17];

									}else if(Str_Reg[n] == Key_Reg[9]){

										Str_Enc[k] = Key_Enc[18];
										Str_Enc[k+1] = Key_Enc[19];

									}else if(Str_Reg[n] == Key_Reg[10]){

										Str_Enc[k] = Key_Enc[20];
										Str_Enc[k+1] = Key_Enc[21];

									}else if(Str_Reg[n] == Key_Reg[11]){

										Str_Enc[k] = Key_Enc[22];
										Str_Enc[k+1] = Key_Enc[23];

									}else if(Str_Reg[n] == Key_Reg[12]){

										Str_Enc[k] = Key_Enc[24];
										Str_Enc[k+1] = Key_Enc[25];

									}else if(Str_Reg[n] == Key_Reg[13]){

										Str_Enc[k] = Key_Enc[26];
										Str_Enc[k+1] = Key_Enc[27];

									}else if(Str_Reg[n] == Key_Reg[14]){

										Str_Enc[k] = Key_Enc[28];
										Str_Enc[k+1] = Key_Enc[29];

									}else if(Str_Reg[n] == Key_Reg[15]){

										Str_Enc[k] = Key_Enc[30];
										Str_Enc[k+1] = Key_Enc[31];

									}else if(Str_Reg[n] == Key_Reg[16]){

										Str_Enc[k] = Key_Enc[32];
										Str_Enc[k+1] = Key_Enc[33];

									}else if(Str_Reg[n] == Key_Reg[17]){

										Str_Enc[k] = Key_Enc[34];
										Str_Enc[k+1] = Key_Enc[35];

									}else if(Str_Reg[n] == Key_Reg[18]){

										Str_Enc[k] = Key_Enc[36];
										Str_Enc[k+1] = Key_Enc[37];

									}else if(Str_Reg[n] == Key_Reg[19]){

										Str_Enc[k] = Key_Enc[38];
										Str_Enc[k+1] = Key_Enc[39];

									}else if(Str_Reg[n] == Key_Reg[20]){

										Str_Enc[k] = Key_Enc[40];
										Str_Enc[k+1] = Key_Enc[41];

									}else if(Str_Reg[n] == Key_Reg[21]){

										Str_Enc[k] = Key_Enc[42];
										Str_Enc[k+1] = Key_Enc[43];

									}else if(Str_Reg[n] == Key_Reg[22]){

										Str_Enc[k] = Key_Enc[44];
										Str_Enc[k+1] = Key_Enc[45];

									}else if(Str_Reg[n] == Key_Reg[23]){

										Str_Enc[k] = Key_Enc[46];
										Str_Enc[k+1] = Key_Enc[47];

									}else if(Str_Reg[n] == Key_Reg[24]){

										Str_Enc[k] = Key_Enc[48];
										Str_Enc[k+1] = Key_Enc[49];

									}else if(Str_Reg[n] == Key_Reg[25]){

										Str_Enc[k] = Key_Enc[50];
										Str_Enc[k+1] = Key_Enc[51];

									}else if(Str_Reg[n] == Key_Reg[26]){

										Str_Enc[k] = Key_Enc[52];
										Str_Enc[k+1] = Key_Enc[53];

									}else if(Str_Reg[n] == Key_Reg[27]){

										Str_Enc[k] = Key_Enc[54];
										Str_Enc[k+1] = Key_Enc[55];

									}else if(Str_Reg[n] == Key_Reg[28]){

										Str_Enc[k] = Key_Enc[56];
										Str_Enc[k+1] = Key_Enc[57];

									}else if(Str_Reg[n] == Key_Reg[29]){

										Str_Enc[k] = Key_Enc[58];
										Str_Enc[k+1] = Key_Enc[59];

									}else if(Str_Reg[n] == Key_Reg[30]){

										Str_Enc[k] = Key_Enc[60];
										Str_Enc[k+1] = Key_Enc[61];

									}else if(Str_Reg[n] == Key_Reg[31]){

										Str_Enc[k] = Key_Enc[62];
										Str_Enc[k+1] = Key_Enc[63];

									}else if(Str_Reg[n] == Key_Reg[32]){

										Str_Enc[k] = Key_Enc[64];
										Str_Enc[k+1] = Key_Enc[65];

									}else if(Str_Reg[n] == Key_Reg[33]){

										Str_Enc[k] = Key_Enc[66];
										Str_Enc[k+1] = Key_Enc[67];

									}else if(Str_Reg[n] == Key_Reg[34]){

										Str_Enc[k] = Key_Enc[68];
										Str_Enc[k+1] = Key_Enc[69];

									}else if(Str_Reg[n] == Key_Reg[35]){

										Str_Enc[k] = Key_Enc[70];
										Str_Enc[k+1] = Key_Enc[71];

									}else if(Str_Reg[n] == Key_Reg[36]){

										Str_Enc[k] = Key_Enc[72];
										Str_Enc[k+1] = Key_Enc[73];

									}else if(Str_Reg[n] == Key_Reg[37]){

										Str_Enc[k] = Key_Enc[74];
										Str_Enc[k+1] = Key_Enc[75];

									}else if(Str_Reg[n] == Key_Reg[38]){

										Str_Enc[k] = Key_Enc[76];
										Str_Enc[k+1] = Key_Enc[77];

									}else if(Str_Reg[n] == Key_Reg[39]){

										Str_Enc[k] = Key_Enc[78];
										Str_Enc[k+1] = Key_Enc[79];

									}else if(Str_Reg[n] == Key_Reg[40]){

										Str_Enc[k] = Key_Enc[80];
										Str_Enc[k+1] = Key_Enc[81];

									}else if(Str_Reg[n] == Key_Reg[41]){

										Str_Enc[k] = Key_Enc[82];
										Str_Enc[k+1] = Key_Enc[83];

									}else if(Str_Reg[n] == Key_Reg[42]){

										Str_Enc[k] = Key_Enc[84];
										Str_Enc[k+1] = Key_Enc[85];

									}else if(Str_Reg[n] == Key_Reg[43]){

										Str_Enc[k] = Key_Enc[86];
										Str_Enc[k+1] = Key_Enc[87];

									}else if(Str_Reg[n] == Key_Reg[44]){

										Str_Enc[k] = Key_Enc[88];
										Str_Enc[k+1] = Key_Enc[89];

									}else if(Str_Reg[n] == Key_Reg[45]){

										Str_Enc[k] = Key_Enc[90];
										Str_Enc[k+1] = Key_Enc[91];

									}else if(Str_Reg[n] == Key_Reg[46]){

										Str_Enc[k] = Key_Enc[92];
										Str_Enc[k+1] = Key_Enc[93];

									}else if(Str_Reg[n] == Key_Reg[47]){

										Str_Enc[k] = Key_Enc[94];
										Str_Enc[k+1] = Key_Enc[95];

									}else if(Str_Reg[n] == Key_Reg[48]){

										Str_Enc[k] = Key_Enc[96];
										Str_Enc[k+1] = Key_Enc[97];

									}else if(Str_Reg[n] == Key_Reg[49]){

										Str_Enc[k] = Key_Enc[98];
										Str_Enc[k+1] = Key_Enc[99];

									}else if(Str_Reg[n] == Key_Reg[50]){

										Str_Enc[k] = Key_Enc[100];
										Str_Enc[k+1] = Key_Enc[101];

									}else if(Str_Reg[n] == Key_Reg[51]){

										Str_Enc[k] = Key_Enc[102];
										Str_Enc[k+1] = Key_Enc[103];

									}else if(Str_Reg[n] == Key_Reg[52]){

										Str_Enc[k] = Key_Enc[104];
										Str_Enc[k+1] = Key_Enc[105];

									}else if(Str_Reg[n] == Key_Reg[53]){

										Str_Enc[k] = Key_Enc[106];
										Str_Enc[k+1] = Key_Enc[107];

									}else if(Str_Reg[n] == Key_Reg[54]){

										Str_Enc[k] = Key_Enc[108];
										Str_Enc[k+1] = Key_Enc[109];

									}else if(Str_Reg[n] == Key_Reg[55]){

										Str_Enc[k] = Key_Enc[110];
										Str_Enc[k+1] = Key_Enc[111];

									}else if(Str_Reg[n] == Key_Reg[56]){

										Str_Enc[k] = Key_Enc[112];
										Str_Enc[k+1] = Key_Enc[113];

									}else if(Str_Reg[n] == Key_Reg[57]){

										Str_Enc[k] = Key_Enc[114];
										Str_Enc[k+1] = Key_Enc[115];

									}else if(Str_Reg[n] == Key_Reg[58]){

										Str_Enc[k] = Key_Enc[116];
										Str_Enc[k+1] = Key_Enc[117];

									}else if(Str_Reg[n] == Key_Reg[59]){

										Str_Enc[k] = Key_Enc[118];
										Str_Enc[k+1] = Key_Enc[119];

									}else if(Str_Reg[n] == Key_Reg[60]){

										Str_Enc[k] = Key_Enc[120];
										Str_Enc[k+1] = Key_Enc[121];

									}else if(Str_Reg[n] == Key_Reg[61]){

										Str_Enc[k] = Key_Enc[122];
										Str_Enc[k+1] = Key_Enc[123];

									}else if(Str_Reg[n] == Key_Reg[62]){

										Str_Enc[k] = Key_Enc[124];
										Str_Enc[k+1] = Key_Enc[125];

									}else if(Str_Reg[n] == Key_Reg[63]){

										Str_Enc[k] = Key_Enc[126];
										Str_Enc[k+1] = Key_Enc[127];

									}

									n = n+1;
									k = k+2;

								}

								printf("\n");
								printf("-----------");
								printf("\n-ENCRYPTED-");
								printf("\n-----------");
								printf("\n\n");

								Strlen_Enc = strlen(Str_Enc);

								for(k=0;k<Strlen_Enc;k++){
									printf("%c",Str_Enc[k]);
									Str_Enc[k]=Ept[k];
									Str_Reg[k]=Ept[k];
								}

								scanf("%c",&v);

			}else if(Key == 4){

				system("cls");

				char Key_Reg[65] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m',
													'n','o','p','q','r','s','t','u','v','w','x','y','z',' ','1','2','3','4','5','6','7','8','9','0','.'};

				char Key_Enc[129] = {'%','u','<','i','$','t',',','n','#','s','>','k','@','r','.','l','!','q','?','+','`','=','/','{','~','-','e','[','a','_','d','}','z',')','b',']','y','(','c',
										'|','x','*','f',':','&','w',';','g','^','v','"','h','u','%','i','<','t','$','n',',','s','#','k','>','r','@','l','.','q','!','+','?','=','`','{','/','-','~',
										'[','e','_','a','}','d',')','z',']','b','(','y','|','c','*','x',':','f','w','&','g',';','v','^','h','"','$','$','9','!','!','8','7','!','!','6','5','!','!',
										'4','3','!','!','2','1','!','!','!','{','}'};

								int Strlen_Enc = 0, Strlen_Reg = 0, n=0, k=0;
								char v;
								char Ept[8000];
								char Str_Reg[4000];
								char Str_Enc[8000];

								printf("    ~~~~~~~~~~~~~~~~~~~");
								printf("\n    ENCRYPTION TERMINAL");
								printf("\n    ~~~~~~~~~~~~~~~~~~~");
								printf("\n******************************************");
								printf("\nEnter the text you want to encrypt below:-");
								printf("\n******************************************");
								printf("\n");
								printf("---------");
								printf("\n-REGULAR-");
								printf("\n---------");
								printf("\n\n");

								scanf("%c",&v);
								gets(Str_Reg);

								Strlen_Reg = strlen(Str_Reg);

								while(n != Strlen_Reg){

									if(Str_Reg[n] == Key_Reg[0]){

										Str_Enc[k] = Key_Enc[0];
										Str_Enc[k+1] = Key_Enc[1];

									}else if(Str_Reg[n] == Key_Reg[1]){

										Str_Enc[k] = Key_Enc[2];
										Str_Enc[k+1] = Key_Enc[3];

									}else if(Str_Reg[n] == Key_Reg[2]){

										Str_Enc[k] = Key_Enc[4];
										Str_Enc[k+1] = Key_Enc[5];

									}else if(Str_Reg[n] == Key_Reg[3]){

										Str_Enc[k] = Key_Enc[6];
										Str_Enc[k+1] = Key_Enc[7];

									}else if(Str_Reg[n] == Key_Reg[4]){

										Str_Enc[k] = Key_Enc[8];
										Str_Enc[k+1] = Key_Enc[9];

									}else if(Str_Reg[n] == Key_Reg[5]){

										Str_Enc[k] = Key_Enc[10];
										Str_Enc[k+1] = Key_Enc[11];

									}else if(Str_Reg[n] == Key_Reg[6]){

										Str_Enc[k] = Key_Enc[12];
										Str_Enc[k+1] = Key_Enc[13];

									}else if(Str_Reg[n] == Key_Reg[7]){

										Str_Enc[k] = Key_Enc[14];
										Str_Enc[k+1] = Key_Enc[15];

									}else if(Str_Reg[n] == Key_Reg[8]){

										Str_Enc[k] = Key_Enc[16];
										Str_Enc[k+1] = Key_Enc[17];

									}else if(Str_Reg[n] == Key_Reg[9]){

										Str_Enc[k] = Key_Enc[18];
										Str_Enc[k+1] = Key_Enc[19];

									}else if(Str_Reg[n] == Key_Reg[10]){

										Str_Enc[k] = Key_Enc[20];
										Str_Enc[k+1] = Key_Enc[21];

									}else if(Str_Reg[n] == Key_Reg[11]){

										Str_Enc[k] = Key_Enc[22];
										Str_Enc[k+1] = Key_Enc[23];

									}else if(Str_Reg[n] == Key_Reg[12]){

										Str_Enc[k] = Key_Enc[24];
										Str_Enc[k+1] = Key_Enc[25];

									}else if(Str_Reg[n] == Key_Reg[13]){

										Str_Enc[k] = Key_Enc[26];
										Str_Enc[k+1] = Key_Enc[27];

									}else if(Str_Reg[n] == Key_Reg[14]){

										Str_Enc[k] = Key_Enc[28];
										Str_Enc[k+1] = Key_Enc[29];

									}else if(Str_Reg[n] == Key_Reg[15]){

										Str_Enc[k] = Key_Enc[30];
										Str_Enc[k+1] = Key_Enc[31];

									}else if(Str_Reg[n] == Key_Reg[16]){

										Str_Enc[k] = Key_Enc[32];
										Str_Enc[k+1] = Key_Enc[33];

									}else if(Str_Reg[n] == Key_Reg[17]){

										Str_Enc[k] = Key_Enc[34];
										Str_Enc[k+1] = Key_Enc[35];

									}else if(Str_Reg[n] == Key_Reg[18]){

										Str_Enc[k] = Key_Enc[36];
										Str_Enc[k+1] = Key_Enc[37];

									}else if(Str_Reg[n] == Key_Reg[19]){

										Str_Enc[k] = Key_Enc[38];
										Str_Enc[k+1] = Key_Enc[39];

									}else if(Str_Reg[n] == Key_Reg[20]){

										Str_Enc[k] = Key_Enc[40];
										Str_Enc[k+1] = Key_Enc[41];

									}else if(Str_Reg[n] == Key_Reg[21]){

										Str_Enc[k] = Key_Enc[42];
										Str_Enc[k+1] = Key_Enc[43];

									}else if(Str_Reg[n] == Key_Reg[22]){

										Str_Enc[k] = Key_Enc[44];
										Str_Enc[k+1] = Key_Enc[45];

									}else if(Str_Reg[n] == Key_Reg[23]){

										Str_Enc[k] = Key_Enc[46];
										Str_Enc[k+1] = Key_Enc[47];

									}else if(Str_Reg[n] == Key_Reg[24]){

										Str_Enc[k] = Key_Enc[48];
										Str_Enc[k+1] = Key_Enc[49];

									}else if(Str_Reg[n] == Key_Reg[25]){

										Str_Enc[k] = Key_Enc[50];
										Str_Enc[k+1] = Key_Enc[51];

									}else if(Str_Reg[n] == Key_Reg[26]){

										Str_Enc[k] = Key_Enc[52];
										Str_Enc[k+1] = Key_Enc[53];

									}else if(Str_Reg[n] == Key_Reg[27]){

										Str_Enc[k] = Key_Enc[54];
										Str_Enc[k+1] = Key_Enc[55];

									}else if(Str_Reg[n] == Key_Reg[28]){

										Str_Enc[k] = Key_Enc[56];
										Str_Enc[k+1] = Key_Enc[57];

									}else if(Str_Reg[n] == Key_Reg[29]){

										Str_Enc[k] = Key_Enc[58];
										Str_Enc[k+1] = Key_Enc[59];

									}else if(Str_Reg[n] == Key_Reg[30]){

										Str_Enc[k] = Key_Enc[60];
										Str_Enc[k+1] = Key_Enc[61];

									}else if(Str_Reg[n] == Key_Reg[31]){

										Str_Enc[k] = Key_Enc[62];
										Str_Enc[k+1] = Key_Enc[63];

									}else if(Str_Reg[n] == Key_Reg[32]){

										Str_Enc[k] = Key_Enc[64];
										Str_Enc[k+1] = Key_Enc[65];

									}else if(Str_Reg[n] == Key_Reg[33]){

										Str_Enc[k] = Key_Enc[66];
										Str_Enc[k+1] = Key_Enc[67];

									}else if(Str_Reg[n] == Key_Reg[34]){

										Str_Enc[k] = Key_Enc[68];
										Str_Enc[k+1] = Key_Enc[69];

									}else if(Str_Reg[n] == Key_Reg[35]){

										Str_Enc[k] = Key_Enc[70];
										Str_Enc[k+1] = Key_Enc[71];

									}else if(Str_Reg[n] == Key_Reg[36]){

										Str_Enc[k] = Key_Enc[72];
										Str_Enc[k+1] = Key_Enc[73];

									}else if(Str_Reg[n] == Key_Reg[37]){

										Str_Enc[k] = Key_Enc[74];
										Str_Enc[k+1] = Key_Enc[75];

									}else if(Str_Reg[n] == Key_Reg[38]){

										Str_Enc[k] = Key_Enc[76];
										Str_Enc[k+1] = Key_Enc[77];

									}else if(Str_Reg[n] == Key_Reg[39]){

										Str_Enc[k] = Key_Enc[78];
										Str_Enc[k+1] = Key_Enc[79];

									}else if(Str_Reg[n] == Key_Reg[40]){

										Str_Enc[k] = Key_Enc[80];
										Str_Enc[k+1] = Key_Enc[81];

									}else if(Str_Reg[n] == Key_Reg[41]){

										Str_Enc[k] = Key_Enc[82];
										Str_Enc[k+1] = Key_Enc[83];

									}else if(Str_Reg[n] == Key_Reg[42]){

										Str_Enc[k] = Key_Enc[84];
										Str_Enc[k+1] = Key_Enc[85];

									}else if(Str_Reg[n] == Key_Reg[43]){

										Str_Enc[k] = Key_Enc[86];
										Str_Enc[k+1] = Key_Enc[87];

									}else if(Str_Reg[n] == Key_Reg[44]){

										Str_Enc[k] = Key_Enc[88];
										Str_Enc[k+1] = Key_Enc[89];

									}else if(Str_Reg[n] == Key_Reg[45]){

										Str_Enc[k] = Key_Enc[90];
										Str_Enc[k+1] = Key_Enc[91];

									}else if(Str_Reg[n] == Key_Reg[46]){

										Str_Enc[k] = Key_Enc[92];
										Str_Enc[k+1] = Key_Enc[93];

									}else if(Str_Reg[n] == Key_Reg[47]){

										Str_Enc[k] = Key_Enc[94];
										Str_Enc[k+1] = Key_Enc[95];

									}else if(Str_Reg[n] == Key_Reg[48]){

										Str_Enc[k] = Key_Enc[96];
										Str_Enc[k+1] = Key_Enc[97];

									}else if(Str_Reg[n] == Key_Reg[49]){

										Str_Enc[k] = Key_Enc[98];
										Str_Enc[k+1] = Key_Enc[99];

									}else if(Str_Reg[n] == Key_Reg[50]){

										Str_Enc[k] = Key_Enc[100];
										Str_Enc[k+1] = Key_Enc[101];

									}else if(Str_Reg[n] == Key_Reg[51]){

										Str_Enc[k] = Key_Enc[102];
										Str_Enc[k+1] = Key_Enc[103];

									}else if(Str_Reg[n] == Key_Reg[52]){

										Str_Enc[k] = Key_Enc[104];
										Str_Enc[k+1] = Key_Enc[105];

									}else if(Str_Reg[n] == Key_Reg[53]){

										Str_Enc[k] = Key_Enc[106];
										Str_Enc[k+1] = Key_Enc[107];

									}else if(Str_Reg[n] == Key_Reg[54]){

										Str_Enc[k] = Key_Enc[108];
										Str_Enc[k+1] = Key_Enc[109];

									}else if(Str_Reg[n] == Key_Reg[55]){

										Str_Enc[k] = Key_Enc[110];
										Str_Enc[k+1] = Key_Enc[111];

									}else if(Str_Reg[n] == Key_Reg[56]){

										Str_Enc[k] = Key_Enc[112];
										Str_Enc[k+1] = Key_Enc[113];

									}else if(Str_Reg[n] == Key_Reg[57]){

										Str_Enc[k] = Key_Enc[114];
										Str_Enc[k+1] = Key_Enc[115];

									}else if(Str_Reg[n] == Key_Reg[58]){

										Str_Enc[k] = Key_Enc[116];
										Str_Enc[k+1] = Key_Enc[117];

									}else if(Str_Reg[n] == Key_Reg[59]){

										Str_Enc[k] = Key_Enc[118];
										Str_Enc[k+1] = Key_Enc[119];

									}else if(Str_Reg[n] == Key_Reg[60]){

										Str_Enc[k] = Key_Enc[120];
										Str_Enc[k+1] = Key_Enc[121];

									}else if(Str_Reg[n] == Key_Reg[61]){

										Str_Enc[k] = Key_Enc[122];
										Str_Enc[k+1] = Key_Enc[123];

									}else if(Str_Reg[n] == Key_Reg[62]){

										Str_Enc[k] = Key_Enc[124];
										Str_Enc[k+1] = Key_Enc[125];

									}else if(Str_Reg[n] == Key_Reg[63]){

										Str_Enc[k] = Key_Enc[126];
										Str_Enc[k+1] = Key_Enc[127];

									}

									n = n+1;
									k = k+2;

								}

								printf("\n");
								printf("-----------");
								printf("\n-ENCRYPTED-");
								printf("\n-----------");
								printf("\n\n");

								Strlen_Enc = strlen(Str_Enc);

								for(k=0;k<Strlen_Enc;k++){
									printf("%c",Str_Enc[k]);
									Str_Enc[k]=Ept[k];
									Str_Reg[k]=Ept[k];
								}

								scanf("%c",&v);

			}else{

				system("cls");
				printf("[INVALID CHOICE]");
				getch();
				system("cls");

			}

		}else if(Opt == 2){

			printf("\nSelect Decryption Key:-\n");
						printf("[1] KEY 1.\n");
						printf("[2] KEY 2.\n");
						printf("[3] KEY 3.\n");
						printf("[4] KEY 4.\n");
						scanf("%d",&Key);

			if(Key == 1){

				system("cls");

			int n=0, Strlen_Enc;

			char Key_Reg[65] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m',
								'n','o','p','q','r','s','t','u','v','w','x','y','z',' ','1','2','3','4','5','6','7','8','9','0','.'};

			char Key_Enc[129] = {'~','-','/','{','`','=','?','+','!','q','.','l','@','r','>','k','#','s',',','n','$','t','<','i','%','u','"','h','^','v',';','g','&','w','f',':','x','*','c',
												'|','y','(','b',']','z',')','d','}','a','_','e','[','-','~','{','/','=','`','+','?','q','!','l','.','r','@','k','>','s','#','n',',','t','$','i','<','u','%',
												'h','"','v','^','g',';','w','&',':','f','*','x','|','c','(','y',']','b',')','z','}','d','_','a','[','e','$','$','9','!','!','8','7','!','!','6','5','!','!',
												'4','3','!','!','2','1','!','!','!','{','}'};

			char v;
				char Str_Enc[8000];
				char Str_Reg[4000];
				char Ept[8000];

				printf("    ~~~~~~~~~~~~~~~~~~~");
				printf("\n    DECRYPTION TERMINAL");
				printf("\n    ~~~~~~~~~~~~~~~~~~~");
				printf("\n******************************************");
				printf("\nEnter the text you want to decrypt below:-");
				printf("\n******************************************");
				printf("\n");
				printf("-----------");
				printf("\n-ENCRYPTED-");
				printf("\n-----------");
				printf("\n\n");

				scanf("%c",&v);
				gets(Str_Enc);

				Strlen_Enc = strlen(Str_Enc);

				while(n != Strlen_Enc){


							if(Str_Enc[n] == Key_Enc[0] && Str_Enc[n+1] == Key_Enc[1]){

								Str_Reg[n] = Key_Reg[0];

							}else if(Str_Enc[n] == Key_Enc[2] && Str_Enc[n+1] == Key_Enc[3]){

								Str_Reg[n] = Key_Reg[1];

							}else if(Str_Enc[n] == Key_Enc[4] && Str_Enc[n+1] == Key_Enc[5]){

								Str_Reg[n] = Key_Reg[2];

							}else if(Str_Enc[n] == Key_Enc[6] && Str_Enc[n+1] == Key_Enc[7]){

								Str_Reg[n] = Key_Reg[3];

							}else if(Str_Enc[n] == Key_Enc[8] && Str_Enc[n+1] == Key_Enc[9]){

								Str_Reg[n] = Key_Reg[4];

							}else if(Str_Enc[n] == Key_Enc[10] && Str_Enc[n+1] == Key_Enc[11]){

								Str_Reg[n] = Key_Reg[5];

							}else if(Str_Enc[n] == Key_Enc[12] && Str_Enc[n+1] == Key_Enc[13]){

								Str_Reg[n] = Key_Reg[6];

							}else if(Str_Enc[n] == Key_Enc[14] && Str_Enc[n+1] == Key_Enc[15]){

								Str_Reg[n] = Key_Reg[7];

							}else if(Str_Enc[n] == Key_Enc[16] && Str_Enc[n+1] == Key_Enc[17]){

								Str_Reg[n] = Key_Reg[8];

							}else if(Str_Enc[n] == Key_Enc[18] && Str_Enc[n+1] == Key_Enc[19]){

								Str_Reg[n] = Key_Reg[9];

							}else if(Str_Enc[n] == Key_Enc[20] && Str_Enc[n+1] == Key_Enc[21]){

								Str_Reg[n] = Key_Reg[10];

							}else if(Str_Enc[n] == Key_Enc[22] && Str_Enc[n+1] == Key_Enc[23]){

								Str_Reg[n] = Key_Reg[11];

							}else if(Str_Enc[n] == Key_Enc[24] && Str_Enc[n+1] == Key_Enc[25]){

								Str_Reg[n] = Key_Reg[12];

							}else if(Str_Enc[n] == Key_Enc[26] && Str_Enc[n+1] == Key_Enc[27]){

								Str_Reg[n] = Key_Reg[13];

							}else if(Str_Enc[n] == Key_Enc[28] && Str_Enc[n+1] == Key_Enc[29]){

								Str_Reg[n] = Key_Reg[14];

							}else if(Str_Enc[n] == Key_Enc[30] && Str_Enc[n+1] == Key_Enc[31]){

								Str_Reg[n] = Key_Reg[15];

							}else if(Str_Enc[n] == Key_Enc[32] && Str_Enc[n+1] == Key_Enc[33]){

								Str_Reg[n] = Key_Reg[16];

							}else if(Str_Enc[n] == Key_Enc[34] && Str_Enc[n+1] == Key_Enc[35]){

								Str_Reg[n] = Key_Reg[17];

							}else if(Str_Enc[n] == Key_Enc[36] && Str_Enc[n+1] == Key_Enc[37]){

								Str_Reg[n] = Key_Reg[18];

							}else if(Str_Enc[n] == Key_Enc[38] && Str_Enc[n+1] == Key_Enc[39]){

								Str_Reg[n] = Key_Reg[19];

							}else if(Str_Enc[n] == Key_Enc[40] && Str_Enc[n+1] == Key_Enc[41]){

								Str_Reg[n] = Key_Reg[20];

							}else if(Str_Enc[n] == Key_Enc[42] && Str_Enc[n+1] == Key_Enc[43]){

								Str_Reg[n] = Key_Reg[21];

							}else if(Str_Enc[n] == Key_Enc[44] && Str_Enc[n+1] == Key_Enc[45]){

								Str_Reg[n] = Key_Reg[22];

							}else if(Str_Enc[n] == Key_Enc[46] && Str_Enc[n+1] == Key_Enc[47]){

								Str_Reg[n] = Key_Reg[23];

							}else if(Str_Enc[n] == Key_Enc[48] && Str_Enc[n+1] == Key_Enc[49]){

								Str_Reg[n] = Key_Reg[24];

							}else if(Str_Enc[n] == Key_Enc[50] && Str_Enc[n+1] == Key_Enc[51]){

								Str_Reg[n] = Key_Reg[25];

							}else if(Str_Enc[n] == Key_Enc[52] && Str_Enc[n+1] == Key_Enc[53]){

								Str_Reg[n] = Key_Reg[26];

							}else if(Str_Enc[n] == Key_Enc[54] && Str_Enc[n+1] == Key_Enc[55]){

								Str_Reg[n] = Key_Reg[27];

							}else if(Str_Enc[n] == Key_Enc[56] && Str_Enc[n+1] == Key_Enc[57]){

								Str_Reg[n] = Key_Reg[28];

							}else if(Str_Enc[n] == Key_Enc[58] && Str_Enc[n+1] == Key_Enc[59]){

								Str_Reg[n] = Key_Reg[29];

							}else if(Str_Enc[n] == Key_Enc[60] && Str_Enc[n+1] == Key_Enc[61]){

								Str_Reg[n] = Key_Reg[30];

							}else if(Str_Enc[n] == Key_Enc[62] && Str_Enc[n+1] == Key_Enc[63]){

								Str_Reg[n] = Key_Reg[31];

							}else if(Str_Enc[n] == Key_Enc[64] && Str_Enc[n+1] == Key_Enc[65]){

								Str_Reg[n] = Key_Reg[32];

							}else if(Str_Enc[n] == Key_Enc[66] && Str_Enc[n+1] == Key_Enc[67]){

								Str_Reg[n] = Key_Reg[33];

							}else if(Str_Enc[n] == Key_Enc[68] && Str_Enc[n+1] == Key_Enc[69]){

								Str_Reg[n] = Key_Reg[34];

							}else if(Str_Enc[n] == Key_Enc[70] && Str_Enc[n+1] == Key_Enc[71]){

								Str_Reg[n] = Key_Reg[35];

							}else if(Str_Enc[n] == Key_Enc[72] && Str_Enc[n+1] == Key_Enc[73]){

								Str_Reg[n] = Key_Reg[36];

							}else if(Str_Enc[n] == Key_Enc[74] && Str_Enc[n+1] == Key_Enc[75]){

								Str_Reg[n] = Key_Reg[37];

							}else if(Str_Enc[n] == Key_Enc[76] && Str_Enc[n+1] == Key_Enc[77]){

								Str_Reg[n] = Key_Reg[38];

							}else if(Str_Enc[n] == Key_Enc[78] && Str_Enc[n+1] == Key_Enc[79]){

								Str_Reg[n] = Key_Reg[39];

							}else if(Str_Enc[n] == Key_Enc[80] && Str_Enc[n+1] == Key_Enc[81]){

								Str_Reg[n] = Key_Reg[40];

							}else if(Str_Enc[n] == Key_Enc[82] && Str_Enc[n+1] == Key_Enc[83]){

								Str_Reg[n] = Key_Reg[41];

							}else if(Str_Enc[n] == Key_Enc[84] && Str_Enc[n+1] == Key_Enc[85]){

								Str_Reg[n] = Key_Reg[42];

							}else if(Str_Enc[n] == Key_Enc[86] && Str_Enc[n+1] == Key_Enc[87]){

								Str_Reg[n] = Key_Reg[43];

							}else if(Str_Enc[n] == Key_Enc[88] && Str_Enc[n+1] == Key_Enc[89]){

								Str_Reg[n] = Key_Reg[44];

							}else if(Str_Enc[n] == Key_Enc[90] && Str_Enc[n+1] == Key_Enc[91]){

								Str_Reg[n] = Key_Reg[45];

							}else if(Str_Enc[n] == Key_Enc[92] && Str_Enc[n+1] == Key_Enc[93]){

								Str_Reg[n] = Key_Reg[46];

							}else if(Str_Enc[n] == Key_Enc[94] && Str_Enc[n+1] == Key_Enc[95]){

								Str_Reg[n] = Key_Reg[47];

							}else if(Str_Enc[n] == Key_Enc[96] && Str_Enc[n+1] == Key_Enc[97]){

								Str_Reg[n] = Key_Reg[48];

							}else if(Str_Enc[n] == Key_Enc[98] && Str_Enc[n+1] == Key_Enc[99]){

								Str_Reg[n] = Key_Reg[49];

							}else if(Str_Enc[n] == Key_Enc[100] && Str_Enc[n+1] == Key_Enc[101]){

								Str_Reg[n] = Key_Reg[50];

							}else if(Str_Enc[n] == Key_Enc[102] && Str_Enc[n+1] == Key_Enc[103]){

								Str_Reg[n] = Key_Reg[51];

							}else if(Str_Enc[n] == Key_Enc[104] && Str_Enc[n+1] == Key_Enc[105]){

								Str_Reg[n] = Key_Reg[52];

							}else if(Str_Enc[n] == Key_Enc[106] && Str_Enc[n+1] == Key_Enc[107]){

								Str_Reg[n] = Key_Reg[53];

							}else if(Str_Enc[n] == Key_Enc[108] && Str_Enc[n+1] == Key_Enc[109]){

								Str_Reg[n] = Key_Reg[54];

							}else if(Str_Enc[n] == Key_Enc[110] && Str_Enc[n+1] == Key_Enc[111]){

								Str_Reg[n] = Key_Reg[55];

							}else if(Str_Enc[n] == Key_Enc[112] && Str_Enc[n+1] == Key_Enc[113]){

								Str_Reg[n] = Key_Reg[56];

							}else if(Str_Enc[n] == Key_Enc[114] && Str_Enc[n+1] == Key_Enc[115]){

								Str_Reg[n] = Key_Reg[57];

							}else if(Str_Enc[n] == Key_Enc[116] && Str_Enc[n+1] == Key_Enc[117]){

								Str_Reg[n] = Key_Reg[58];

							}else if(Str_Enc[n] == Key_Enc[118] && Str_Enc[n+1] == Key_Enc[119]){

								Str_Reg[n] = Key_Reg[59];

							}else if(Str_Enc[n] == Key_Enc[120] && Str_Enc[n+1] == Key_Enc[121]){

								Str_Reg[n] = Key_Reg[60];

							}else if(Str_Enc[n] == Key_Enc[122] && Str_Enc[n+1] == Key_Enc[123]){

								Str_Reg[n] = Key_Reg[61];

							}else if(Str_Enc[n] == Key_Enc[124] && Str_Enc[n+1] == Key_Enc[125]){

								Str_Reg[n] = Key_Reg[62];

							}else if(Str_Enc[n] == Key_Enc[126] && Str_Enc[n+1] == Key_Enc[127]){

								Str_Reg[n] = Key_Reg[63];

							}

					n = n+2;

				}

				printf("\n");
				printf("-----------");
				printf("\n-DECRYPTED-");
				printf("\n-----------");
				printf("\n\n");

				for(n=0;n!=Strlen_Enc;n++){
					printf("%c",Str_Reg[n]);
					Str_Reg[n]=Ept[n];
					Str_Enc[n]=Ept[n];
					Str_Enc[n+1]=Ept[n+1];
					n++;
				}
				scanf("%c",&v);

			}else if(Key == 2){

				system("cls");

				int n=0, Strlen_Enc;

				char Key_Reg[65] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m',
									'n','o','p','q','r','s','t','u','v','w','x','y','z',' ','1','2','3','4','5','6','7','8','9','0','.'};

				char Key_Enc[129] = {'e','[','a','_','d','}','z',')','b',']','y','(','c','|','x','*','f',':','&','w',';','g','^','v','"','h','%','u','<','i','$','t',',','n','#','s','>','k','@',
														'r','.','l','!','q','?','+','`','=','/','{','~','-','[','e','_','a','}','d',')','z',']','b','(','y','|','c','*','x',':','f','w','&','g',';','v','^','h','"',
														'u','%','i','<','t','$','n',',','s','#','k','>','r','@','l','.','q','!','+','?','=','`','{','/','-','~','$','$','9','!','!','8','7','!','!','6','5','!','!',
														'4','3','!','!','2','1','!','!','!','{','}'};
				char v;
					char Ept[8000];
					char Str_Enc[8000];
					char Str_Reg[4000];

					printf("    ~~~~~~~~~~~~~~~~~~~");
					printf("\n    DECRYPTION TERMINAL");
					printf("\n    ~~~~~~~~~~~~~~~~~~~");
					printf("\n******************************************");
					printf("\nEnter the text you want to decrypt below:-");
					printf("\n******************************************");
					printf("\n");
					printf("-----------");
					printf("\n-ENCRYPTED-");
					printf("\n-----------");
					printf("\n\n");

					scanf("%c",&v);
					gets(Str_Enc);

					Strlen_Enc = strlen(Str_Enc);

					while(n != Strlen_Enc){


								if(Str_Enc[n] == Key_Enc[0] && Str_Enc[n+1] == Key_Enc[1]){

									Str_Reg[n] = Key_Reg[0];

								}else if(Str_Enc[n] == Key_Enc[2] && Str_Enc[n+1] == Key_Enc[3]){

									Str_Reg[n] = Key_Reg[1];

								}else if(Str_Enc[n] == Key_Enc[4] && Str_Enc[n+1] == Key_Enc[5]){

									Str_Reg[n] = Key_Reg[2];

								}else if(Str_Enc[n] == Key_Enc[6] && Str_Enc[n+1] == Key_Enc[7]){

									Str_Reg[n] = Key_Reg[3];

								}else if(Str_Enc[n] == Key_Enc[8] && Str_Enc[n+1] == Key_Enc[9]){

									Str_Reg[n] = Key_Reg[4];

								}else if(Str_Enc[n] == Key_Enc[10] && Str_Enc[n+1] == Key_Enc[11]){

									Str_Reg[n] = Key_Reg[5];

								}else if(Str_Enc[n] == Key_Enc[12] && Str_Enc[n+1] == Key_Enc[13]){

									Str_Reg[n] = Key_Reg[6];

								}else if(Str_Enc[n] == Key_Enc[14] && Str_Enc[n+1] == Key_Enc[15]){

									Str_Reg[n] = Key_Reg[7];

								}else if(Str_Enc[n] == Key_Enc[16] && Str_Enc[n+1] == Key_Enc[17]){

									Str_Reg[n] = Key_Reg[8];

								}else if(Str_Enc[n] == Key_Enc[18] && Str_Enc[n+1] == Key_Enc[19]){

									Str_Reg[n] = Key_Reg[9];

								}else if(Str_Enc[n] == Key_Enc[20] && Str_Enc[n+1] == Key_Enc[21]){

									Str_Reg[n] = Key_Reg[10];

								}else if(Str_Enc[n] == Key_Enc[22] && Str_Enc[n+1] == Key_Enc[23]){

									Str_Reg[n] = Key_Reg[11];

								}else if(Str_Enc[n] == Key_Enc[24] && Str_Enc[n+1] == Key_Enc[25]){

									Str_Reg[n] = Key_Reg[12];

								}else if(Str_Enc[n] == Key_Enc[26] && Str_Enc[n+1] == Key_Enc[27]){

									Str_Reg[n] = Key_Reg[13];

								}else if(Str_Enc[n] == Key_Enc[28] && Str_Enc[n+1] == Key_Enc[29]){

									Str_Reg[n] = Key_Reg[14];

								}else if(Str_Enc[n] == Key_Enc[30] && Str_Enc[n+1] == Key_Enc[31]){

									Str_Reg[n] = Key_Reg[15];

								}else if(Str_Enc[n] == Key_Enc[32] && Str_Enc[n+1] == Key_Enc[33]){

									Str_Reg[n] = Key_Reg[16];

								}else if(Str_Enc[n] == Key_Enc[34] && Str_Enc[n+1] == Key_Enc[35]){

									Str_Reg[n] = Key_Reg[17];

								}else if(Str_Enc[n] == Key_Enc[36] && Str_Enc[n+1] == Key_Enc[37]){

									Str_Reg[n] = Key_Reg[18];

								}else if(Str_Enc[n] == Key_Enc[38] && Str_Enc[n+1] == Key_Enc[39]){

									Str_Reg[n] = Key_Reg[19];

								}else if(Str_Enc[n] == Key_Enc[40] && Str_Enc[n+1] == Key_Enc[41]){

									Str_Reg[n] = Key_Reg[20];

								}else if(Str_Enc[n] == Key_Enc[42] && Str_Enc[n+1] == Key_Enc[43]){

									Str_Reg[n] = Key_Reg[21];

								}else if(Str_Enc[n] == Key_Enc[44] && Str_Enc[n+1] == Key_Enc[45]){

									Str_Reg[n] = Key_Reg[22];

								}else if(Str_Enc[n] == Key_Enc[46] && Str_Enc[n+1] == Key_Enc[47]){

									Str_Reg[n] = Key_Reg[23];

								}else if(Str_Enc[n] == Key_Enc[48] && Str_Enc[n+1] == Key_Enc[49]){

									Str_Reg[n] = Key_Reg[24];

								}else if(Str_Enc[n] == Key_Enc[50] && Str_Enc[n+1] == Key_Enc[51]){

									Str_Reg[n] = Key_Reg[25];

								}else if(Str_Enc[n] == Key_Enc[52] && Str_Enc[n+1] == Key_Enc[53]){

									Str_Reg[n] = Key_Reg[26];

								}else if(Str_Enc[n] == Key_Enc[54] && Str_Enc[n+1] == Key_Enc[55]){

									Str_Reg[n] = Key_Reg[27];

								}else if(Str_Enc[n] == Key_Enc[56] && Str_Enc[n+1] == Key_Enc[57]){

									Str_Reg[n] = Key_Reg[28];

								}else if(Str_Enc[n] == Key_Enc[58] && Str_Enc[n+1] == Key_Enc[59]){

									Str_Reg[n] = Key_Reg[29];

								}else if(Str_Enc[n] == Key_Enc[60] && Str_Enc[n+1] == Key_Enc[61]){

									Str_Reg[n] = Key_Reg[30];

								}else if(Str_Enc[n] == Key_Enc[62] && Str_Enc[n+1] == Key_Enc[63]){

									Str_Reg[n] = Key_Reg[31];

								}else if(Str_Enc[n] == Key_Enc[64] && Str_Enc[n+1] == Key_Enc[65]){

									Str_Reg[n] = Key_Reg[32];

								}else if(Str_Enc[n] == Key_Enc[66] && Str_Enc[n+1] == Key_Enc[67]){

									Str_Reg[n] = Key_Reg[33];

								}else if(Str_Enc[n] == Key_Enc[68] && Str_Enc[n+1] == Key_Enc[69]){

									Str_Reg[n] = Key_Reg[34];

								}else if(Str_Enc[n] == Key_Enc[70] && Str_Enc[n+1] == Key_Enc[71]){

									Str_Reg[n] = Key_Reg[35];

								}else if(Str_Enc[n] == Key_Enc[72] && Str_Enc[n+1] == Key_Enc[73]){

									Str_Reg[n] = Key_Reg[36];

								}else if(Str_Enc[n] == Key_Enc[74] && Str_Enc[n+1] == Key_Enc[75]){

									Str_Reg[n] = Key_Reg[37];

								}else if(Str_Enc[n] == Key_Enc[76] && Str_Enc[n+1] == Key_Enc[77]){

									Str_Reg[n] = Key_Reg[38];

								}else if(Str_Enc[n] == Key_Enc[78] && Str_Enc[n+1] == Key_Enc[79]){

									Str_Reg[n] = Key_Reg[39];

								}else if(Str_Enc[n] == Key_Enc[80] && Str_Enc[n+1] == Key_Enc[81]){

									Str_Reg[n] = Key_Reg[40];

								}else if(Str_Enc[n] == Key_Enc[82] && Str_Enc[n+1] == Key_Enc[83]){

									Str_Reg[n] = Key_Reg[41];

								}else if(Str_Enc[n] == Key_Enc[84] && Str_Enc[n+1] == Key_Enc[85]){

									Str_Reg[n] = Key_Reg[42];

								}else if(Str_Enc[n] == Key_Enc[86] && Str_Enc[n+1] == Key_Enc[87]){

									Str_Reg[n] = Key_Reg[43];

								}else if(Str_Enc[n] == Key_Enc[88] && Str_Enc[n+1] == Key_Enc[89]){

									Str_Reg[n] = Key_Reg[44];

								}else if(Str_Enc[n] == Key_Enc[90] && Str_Enc[n+1] == Key_Enc[91]){

									Str_Reg[n] = Key_Reg[45];

								}else if(Str_Enc[n] == Key_Enc[92] && Str_Enc[n+1] == Key_Enc[93]){

									Str_Reg[n] = Key_Reg[46];

								}else if(Str_Enc[n] == Key_Enc[94] && Str_Enc[n+1] == Key_Enc[95]){

									Str_Reg[n] = Key_Reg[47];

								}else if(Str_Enc[n] == Key_Enc[96] && Str_Enc[n+1] == Key_Enc[97]){

									Str_Reg[n] = Key_Reg[48];

								}else if(Str_Enc[n] == Key_Enc[98] && Str_Enc[n+1] == Key_Enc[99]){

									Str_Reg[n] = Key_Reg[49];

								}else if(Str_Enc[n] == Key_Enc[100] && Str_Enc[n+1] == Key_Enc[101]){

									Str_Reg[n] = Key_Reg[50];

								}else if(Str_Enc[n] == Key_Enc[102] && Str_Enc[n+1] == Key_Enc[103]){

									Str_Reg[n] = Key_Reg[51];

								}else if(Str_Enc[n] == Key_Enc[104] && Str_Enc[n+1] == Key_Enc[105]){

									Str_Reg[n] = Key_Reg[52];

								}else if(Str_Enc[n] == Key_Enc[106] && Str_Enc[n+1] == Key_Enc[107]){

									Str_Reg[n] = Key_Reg[53];

								}else if(Str_Enc[n] == Key_Enc[108] && Str_Enc[n+1] == Key_Enc[109]){

									Str_Reg[n] = Key_Reg[54];

								}else if(Str_Enc[n] == Key_Enc[110] && Str_Enc[n+1] == Key_Enc[111]){

									Str_Reg[n] = Key_Reg[55];

								}else if(Str_Enc[n] == Key_Enc[112] && Str_Enc[n+1] == Key_Enc[113]){

									Str_Reg[n] = Key_Reg[56];

								}else if(Str_Enc[n] == Key_Enc[114] && Str_Enc[n+1] == Key_Enc[115]){

									Str_Reg[n] = Key_Reg[57];

								}else if(Str_Enc[n] == Key_Enc[116] && Str_Enc[n+1] == Key_Enc[117]){

									Str_Reg[n] = Key_Reg[58];

								}else if(Str_Enc[n] == Key_Enc[118] && Str_Enc[n+1] == Key_Enc[119]){

									Str_Reg[n] = Key_Reg[59];

								}else if(Str_Enc[n] == Key_Enc[120] && Str_Enc[n+1] == Key_Enc[121]){

									Str_Reg[n] = Key_Reg[60];

								}else if(Str_Enc[n] == Key_Enc[122] && Str_Enc[n+1] == Key_Enc[123]){

									Str_Reg[n] = Key_Reg[61];

								}else if(Str_Enc[n] == Key_Enc[124] && Str_Enc[n+1] == Key_Enc[125]){

									Str_Reg[n] = Key_Reg[62];

								}else if(Str_Enc[n] == Key_Enc[126] && Str_Enc[n+1] == Key_Enc[127]){

									Str_Reg[n] = Key_Reg[63];

								}

						n = n+2;

					}

					printf("\n");
					printf("-----------");
					printf("\n-DECRYPTED-");
					printf("\n-----------");
					printf("\n\n");

					for(n=0;n!=Strlen_Enc;n++){
						printf("%c",Str_Reg[n]);
						Str_Reg[n]=Ept[n];
						Str_Enc[n]=Ept[n];
						Str_Enc[n+1]=Ept[n+1];
						n++;
					}

					scanf("%c",&v);

			}else if(Key == 3){

				system("cls");

				int n=0, Strlen_Enc;

				char Key_Reg[65] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m',
									'n','o','p','q','r','s','t','u','v','w','x','y','z',' ','1','2','3','4','5','6','7','8','9','0','.'};

				char Key_Enc[129] = {'"','h','^','v',';','g','&','w','f',':','x','*','c','|','y','(','b',']','z',')','d','}','a','_','e','[','~','-','/','{','`','=','?','+','!','q','.','l','@',
														'r','>','k','#','s',',','n','$','t','<','i','%','u','h','"','v','^','g',';','w','&',':','f','*','x','|','c','(','y',']','b',')','z','}','d','_','a','[','e',
														'-','~','{','/','=','`','+','?','q','!','l','.','r','@','k','>','s','#','n',',','t','$','i','<','u','%','$','$','9','!','!','8','7','!','!','6','5','!','!',
														'4','3','!','!','2','1','!','!','!','{','}'};
				char v;
					char Ept[8000];
					char Str_Enc[8000];
					char Str_Reg[4000];

					printf("    ~~~~~~~~~~~~~~~~~~~");
					printf("\n    DECRYPTION TERMINAL");
					printf("\n    ~~~~~~~~~~~~~~~~~~~");
					printf("\n******************************************");
					printf("\nEnter the text you want to decrypt below:-");
					printf("\n******************************************");
					printf("\n");
					printf("-----------");
					printf("\n-ENCRYPTED-");
					printf("\n-----------");
					printf("\n\n");

					scanf("%c",&v);
					gets(Str_Enc);

					Strlen_Enc = strlen(Str_Enc);

					while(n != Strlen_Enc){


								if(Str_Enc[n] == Key_Enc[0] && Str_Enc[n+1] == Key_Enc[1]){

									Str_Reg[n] = Key_Reg[0];

								}else if(Str_Enc[n] == Key_Enc[2] && Str_Enc[n+1] == Key_Enc[3]){

									Str_Reg[n] = Key_Reg[1];

								}else if(Str_Enc[n] == Key_Enc[4] && Str_Enc[n+1] == Key_Enc[5]){

									Str_Reg[n] = Key_Reg[2];

								}else if(Str_Enc[n] == Key_Enc[6] && Str_Enc[n+1] == Key_Enc[7]){

									Str_Reg[n] = Key_Reg[3];

								}else if(Str_Enc[n] == Key_Enc[8] && Str_Enc[n+1] == Key_Enc[9]){

									Str_Reg[n] = Key_Reg[4];

								}else if(Str_Enc[n] == Key_Enc[10] && Str_Enc[n+1] == Key_Enc[11]){

									Str_Reg[n] = Key_Reg[5];

								}else if(Str_Enc[n] == Key_Enc[12] && Str_Enc[n+1] == Key_Enc[13]){

									Str_Reg[n] = Key_Reg[6];

								}else if(Str_Enc[n] == Key_Enc[14] && Str_Enc[n+1] == Key_Enc[15]){

									Str_Reg[n] = Key_Reg[7];

								}else if(Str_Enc[n] == Key_Enc[16] && Str_Enc[n+1] == Key_Enc[17]){

									Str_Reg[n] = Key_Reg[8];

								}else if(Str_Enc[n] == Key_Enc[18] && Str_Enc[n+1] == Key_Enc[19]){

									Str_Reg[n] = Key_Reg[9];

								}else if(Str_Enc[n] == Key_Enc[20] && Str_Enc[n+1] == Key_Enc[21]){

									Str_Reg[n] = Key_Reg[10];

								}else if(Str_Enc[n] == Key_Enc[22] && Str_Enc[n+1] == Key_Enc[23]){

									Str_Reg[n] = Key_Reg[11];

								}else if(Str_Enc[n] == Key_Enc[24] && Str_Enc[n+1] == Key_Enc[25]){

									Str_Reg[n] = Key_Reg[12];

								}else if(Str_Enc[n] == Key_Enc[26] && Str_Enc[n+1] == Key_Enc[27]){

									Str_Reg[n] = Key_Reg[13];

								}else if(Str_Enc[n] == Key_Enc[28] && Str_Enc[n+1] == Key_Enc[29]){

									Str_Reg[n] = Key_Reg[14];

								}else if(Str_Enc[n] == Key_Enc[30] && Str_Enc[n+1] == Key_Enc[31]){

									Str_Reg[n] = Key_Reg[15];

								}else if(Str_Enc[n] == Key_Enc[32] && Str_Enc[n+1] == Key_Enc[33]){

									Str_Reg[n] = Key_Reg[16];

								}else if(Str_Enc[n] == Key_Enc[34] && Str_Enc[n+1] == Key_Enc[35]){

									Str_Reg[n] = Key_Reg[17];

								}else if(Str_Enc[n] == Key_Enc[36] && Str_Enc[n+1] == Key_Enc[37]){

									Str_Reg[n] = Key_Reg[18];

								}else if(Str_Enc[n] == Key_Enc[38] && Str_Enc[n+1] == Key_Enc[39]){

									Str_Reg[n] = Key_Reg[19];

								}else if(Str_Enc[n] == Key_Enc[40] && Str_Enc[n+1] == Key_Enc[41]){

									Str_Reg[n] = Key_Reg[20];

								}else if(Str_Enc[n] == Key_Enc[42] && Str_Enc[n+1] == Key_Enc[43]){

									Str_Reg[n] = Key_Reg[21];

								}else if(Str_Enc[n] == Key_Enc[44] && Str_Enc[n+1] == Key_Enc[45]){

									Str_Reg[n] = Key_Reg[22];

								}else if(Str_Enc[n] == Key_Enc[46] && Str_Enc[n+1] == Key_Enc[47]){

									Str_Reg[n] = Key_Reg[23];

								}else if(Str_Enc[n] == Key_Enc[48] && Str_Enc[n+1] == Key_Enc[49]){

									Str_Reg[n] = Key_Reg[24];

								}else if(Str_Enc[n] == Key_Enc[50] && Str_Enc[n+1] == Key_Enc[51]){

									Str_Reg[n] = Key_Reg[25];

								}else if(Str_Enc[n] == Key_Enc[52] && Str_Enc[n+1] == Key_Enc[53]){

									Str_Reg[n] = Key_Reg[26];

								}else if(Str_Enc[n] == Key_Enc[54] && Str_Enc[n+1] == Key_Enc[55]){

									Str_Reg[n] = Key_Reg[27];

								}else if(Str_Enc[n] == Key_Enc[56] && Str_Enc[n+1] == Key_Enc[57]){

									Str_Reg[n] = Key_Reg[28];

								}else if(Str_Enc[n] == Key_Enc[58] && Str_Enc[n+1] == Key_Enc[59]){

									Str_Reg[n] = Key_Reg[29];

								}else if(Str_Enc[n] == Key_Enc[60] && Str_Enc[n+1] == Key_Enc[61]){

									Str_Reg[n] = Key_Reg[30];

								}else if(Str_Enc[n] == Key_Enc[62] && Str_Enc[n+1] == Key_Enc[63]){

									Str_Reg[n] = Key_Reg[31];

								}else if(Str_Enc[n] == Key_Enc[64] && Str_Enc[n+1] == Key_Enc[65]){

									Str_Reg[n] = Key_Reg[32];

								}else if(Str_Enc[n] == Key_Enc[66] && Str_Enc[n+1] == Key_Enc[67]){

									Str_Reg[n] = Key_Reg[33];

								}else if(Str_Enc[n] == Key_Enc[68] && Str_Enc[n+1] == Key_Enc[69]){

									Str_Reg[n] = Key_Reg[34];

								}else if(Str_Enc[n] == Key_Enc[70] && Str_Enc[n+1] == Key_Enc[71]){

									Str_Reg[n] = Key_Reg[35];

								}else if(Str_Enc[n] == Key_Enc[72] && Str_Enc[n+1] == Key_Enc[73]){

									Str_Reg[n] = Key_Reg[36];

								}else if(Str_Enc[n] == Key_Enc[74] && Str_Enc[n+1] == Key_Enc[75]){

									Str_Reg[n] = Key_Reg[37];

								}else if(Str_Enc[n] == Key_Enc[76] && Str_Enc[n+1] == Key_Enc[77]){

									Str_Reg[n] = Key_Reg[38];

								}else if(Str_Enc[n] == Key_Enc[78] && Str_Enc[n+1] == Key_Enc[79]){

									Str_Reg[n] = Key_Reg[39];

								}else if(Str_Enc[n] == Key_Enc[80] && Str_Enc[n+1] == Key_Enc[81]){

									Str_Reg[n] = Key_Reg[40];

								}else if(Str_Enc[n] == Key_Enc[82] && Str_Enc[n+1] == Key_Enc[83]){

									Str_Reg[n] = Key_Reg[41];

								}else if(Str_Enc[n] == Key_Enc[84] && Str_Enc[n+1] == Key_Enc[85]){

									Str_Reg[n] = Key_Reg[42];

								}else if(Str_Enc[n] == Key_Enc[86] && Str_Enc[n+1] == Key_Enc[87]){

									Str_Reg[n] = Key_Reg[43];

								}else if(Str_Enc[n] == Key_Enc[88] && Str_Enc[n+1] == Key_Enc[89]){

									Str_Reg[n] = Key_Reg[44];

								}else if(Str_Enc[n] == Key_Enc[90] && Str_Enc[n+1] == Key_Enc[91]){

									Str_Reg[n] = Key_Reg[45];

								}else if(Str_Enc[n] == Key_Enc[92] && Str_Enc[n+1] == Key_Enc[93]){

									Str_Reg[n] = Key_Reg[46];

								}else if(Str_Enc[n] == Key_Enc[94] && Str_Enc[n+1] == Key_Enc[95]){

									Str_Reg[n] = Key_Reg[47];

								}else if(Str_Enc[n] == Key_Enc[96] && Str_Enc[n+1] == Key_Enc[97]){

									Str_Reg[n] = Key_Reg[48];

								}else if(Str_Enc[n] == Key_Enc[98] && Str_Enc[n+1] == Key_Enc[99]){

									Str_Reg[n] = Key_Reg[49];

								}else if(Str_Enc[n] == Key_Enc[100] && Str_Enc[n+1] == Key_Enc[101]){

									Str_Reg[n] = Key_Reg[50];

								}else if(Str_Enc[n] == Key_Enc[102] && Str_Enc[n+1] == Key_Enc[103]){

									Str_Reg[n] = Key_Reg[51];

								}else if(Str_Enc[n] == Key_Enc[104] && Str_Enc[n+1] == Key_Enc[105]){

									Str_Reg[n] = Key_Reg[52];

								}else if(Str_Enc[n] == Key_Enc[106] && Str_Enc[n+1] == Key_Enc[107]){

									Str_Reg[n] = Key_Reg[53];

								}else if(Str_Enc[n] == Key_Enc[108] && Str_Enc[n+1] == Key_Enc[109]){

									Str_Reg[n] = Key_Reg[54];

								}else if(Str_Enc[n] == Key_Enc[110] && Str_Enc[n+1] == Key_Enc[111]){

									Str_Reg[n] = Key_Reg[55];

								}else if(Str_Enc[n] == Key_Enc[112] && Str_Enc[n+1] == Key_Enc[113]){

									Str_Reg[n] = Key_Reg[56];

								}else if(Str_Enc[n] == Key_Enc[114] && Str_Enc[n+1] == Key_Enc[115]){

									Str_Reg[n] = Key_Reg[57];

								}else if(Str_Enc[n] == Key_Enc[116] && Str_Enc[n+1] == Key_Enc[117]){

									Str_Reg[n] = Key_Reg[58];

								}else if(Str_Enc[n] == Key_Enc[118] && Str_Enc[n+1] == Key_Enc[119]){

									Str_Reg[n] = Key_Reg[59];

								}else if(Str_Enc[n] == Key_Enc[120] && Str_Enc[n+1] == Key_Enc[121]){

									Str_Reg[n] = Key_Reg[60];

								}else if(Str_Enc[n] == Key_Enc[122] && Str_Enc[n+1] == Key_Enc[123]){

									Str_Reg[n] = Key_Reg[61];

								}else if(Str_Enc[n] == Key_Enc[124] && Str_Enc[n+1] == Key_Enc[125]){

									Str_Reg[n] = Key_Reg[62];

								}else if(Str_Enc[n] == Key_Enc[126] && Str_Enc[n+1] == Key_Enc[127]){

									Str_Reg[n] = Key_Reg[63];

								}

						n = n+2;

					}

					printf("\n");
					printf("-----------");
					printf("\n-DECRYPTED-");
					printf("\n-----------");
					printf("\n\n");

					for(n=0;n!=Strlen_Enc;n++){
						printf("%c",Str_Reg[n]);
						Str_Reg[n]=Ept[n];
						Str_Enc[n]=Ept[n];
						Str_Enc[n+1]=Ept[n+1];
						n++;
					}

					scanf("%c",&v);

			}else if(Key == 4){

				system("cls");

				int n=0, Strlen_Enc;

				char Key_Reg[65] = {'A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m',
									'n','o','p','q','r','s','t','u','v','w','x','y','z',' ','1','2','3','4','5','6','7','8','9','0','.'};

				char Key_Enc[129] = {'%','u','<','i','$','t',',','n','#','s','>','k','@','r','.','l','!','q','?','+','`','=','/','{','~','-','e','[','a','_','d','}','z',')','b',']','y','(','c',
														'|','x','*','f',':','&','w',';','g','^','v','"','h','u','%','i','<','t','$','n',',','s','#','k','>','r','@','l','.','q','!','+','?','=','`','{','/','-','~',
														'[','e','_','a','}','d',')','z',']','b','(','y','|','c','*','x',':','f','w','&','g',';','v','^','h','"','$','$','9','!','!','8','7','!','!','6','5','!','!',
														'4','3','!','!','2','1','!','!','!','{','}'};
				char v;
					char Ept[8000];
					char Str_Enc[8000];
					char Str_Reg[4000];

					printf("    ~~~~~~~~~~~~~~~~~~~");
					printf("\n    DECRYPTION TERMINAL");
					printf("\n    ~~~~~~~~~~~~~~~~~~~");
					printf("\n******************************************");
					printf("\nEnter the text you want to decrypt below:-");
					printf("\n******************************************");
					printf("\n");
					printf("-----------");
					printf("\n-ENCRYPTED-");
					printf("\n-----------");
					printf("\n\n");

					scanf("%c",&v);
					gets(Str_Enc);

					Strlen_Enc = strlen(Str_Enc);

					while(n != Strlen_Enc){


								if(Str_Enc[n] == Key_Enc[0] && Str_Enc[n+1] == Key_Enc[1]){

									Str_Reg[n] = Key_Reg[0];

								}else if(Str_Enc[n] == Key_Enc[2] && Str_Enc[n+1] == Key_Enc[3]){

									Str_Reg[n] = Key_Reg[1];

								}else if(Str_Enc[n] == Key_Enc[4] && Str_Enc[n+1] == Key_Enc[5]){

									Str_Reg[n] = Key_Reg[2];

								}else if(Str_Enc[n] == Key_Enc[6] && Str_Enc[n+1] == Key_Enc[7]){

									Str_Reg[n] = Key_Reg[3];

								}else if(Str_Enc[n] == Key_Enc[8] && Str_Enc[n+1] == Key_Enc[9]){

									Str_Reg[n] = Key_Reg[4];

								}else if(Str_Enc[n] == Key_Enc[10] && Str_Enc[n+1] == Key_Enc[11]){

									Str_Reg[n] = Key_Reg[5];

								}else if(Str_Enc[n] == Key_Enc[12] && Str_Enc[n+1] == Key_Enc[13]){

									Str_Reg[n] = Key_Reg[6];

								}else if(Str_Enc[n] == Key_Enc[14] && Str_Enc[n+1] == Key_Enc[15]){

									Str_Reg[n] = Key_Reg[7];

								}else if(Str_Enc[n] == Key_Enc[16] && Str_Enc[n+1] == Key_Enc[17]){

									Str_Reg[n] = Key_Reg[8];

								}else if(Str_Enc[n] == Key_Enc[18] && Str_Enc[n+1] == Key_Enc[19]){

									Str_Reg[n] = Key_Reg[9];

								}else if(Str_Enc[n] == Key_Enc[20] && Str_Enc[n+1] == Key_Enc[21]){

									Str_Reg[n] = Key_Reg[10];

								}else if(Str_Enc[n] == Key_Enc[22] && Str_Enc[n+1] == Key_Enc[23]){

									Str_Reg[n] = Key_Reg[11];

								}else if(Str_Enc[n] == Key_Enc[24] && Str_Enc[n+1] == Key_Enc[25]){

									Str_Reg[n] = Key_Reg[12];

								}else if(Str_Enc[n] == Key_Enc[26] && Str_Enc[n+1] == Key_Enc[27]){

									Str_Reg[n] = Key_Reg[13];

								}else if(Str_Enc[n] == Key_Enc[28] && Str_Enc[n+1] == Key_Enc[29]){

									Str_Reg[n] = Key_Reg[14];

								}else if(Str_Enc[n] == Key_Enc[30] && Str_Enc[n+1] == Key_Enc[31]){

									Str_Reg[n] = Key_Reg[15];

								}else if(Str_Enc[n] == Key_Enc[32] && Str_Enc[n+1] == Key_Enc[33]){

									Str_Reg[n] = Key_Reg[16];

								}else if(Str_Enc[n] == Key_Enc[34] && Str_Enc[n+1] == Key_Enc[35]){

									Str_Reg[n] = Key_Reg[17];

								}else if(Str_Enc[n] == Key_Enc[36] && Str_Enc[n+1] == Key_Enc[37]){

									Str_Reg[n] = Key_Reg[18];

								}else if(Str_Enc[n] == Key_Enc[38] && Str_Enc[n+1] == Key_Enc[39]){

									Str_Reg[n] = Key_Reg[19];

								}else if(Str_Enc[n] == Key_Enc[40] && Str_Enc[n+1] == Key_Enc[41]){

									Str_Reg[n] = Key_Reg[20];

								}else if(Str_Enc[n] == Key_Enc[42] && Str_Enc[n+1] == Key_Enc[43]){

									Str_Reg[n] = Key_Reg[21];

								}else if(Str_Enc[n] == Key_Enc[44] && Str_Enc[n+1] == Key_Enc[45]){

									Str_Reg[n] = Key_Reg[22];

								}else if(Str_Enc[n] == Key_Enc[46] && Str_Enc[n+1] == Key_Enc[47]){

									Str_Reg[n] = Key_Reg[23];

								}else if(Str_Enc[n] == Key_Enc[48] && Str_Enc[n+1] == Key_Enc[49]){

									Str_Reg[n] = Key_Reg[24];

								}else if(Str_Enc[n] == Key_Enc[50] && Str_Enc[n+1] == Key_Enc[51]){

									Str_Reg[n] = Key_Reg[25];

								}else if(Str_Enc[n] == Key_Enc[52] && Str_Enc[n+1] == Key_Enc[53]){

									Str_Reg[n] = Key_Reg[26];

								}else if(Str_Enc[n] == Key_Enc[54] && Str_Enc[n+1] == Key_Enc[55]){

									Str_Reg[n] = Key_Reg[27];

								}else if(Str_Enc[n] == Key_Enc[56] && Str_Enc[n+1] == Key_Enc[57]){

									Str_Reg[n] = Key_Reg[28];

								}else if(Str_Enc[n] == Key_Enc[58] && Str_Enc[n+1] == Key_Enc[59]){

									Str_Reg[n] = Key_Reg[29];

								}else if(Str_Enc[n] == Key_Enc[60] && Str_Enc[n+1] == Key_Enc[61]){

									Str_Reg[n] = Key_Reg[30];

								}else if(Str_Enc[n] == Key_Enc[62] && Str_Enc[n+1] == Key_Enc[63]){

									Str_Reg[n] = Key_Reg[31];

								}else if(Str_Enc[n] == Key_Enc[64] && Str_Enc[n+1] == Key_Enc[65]){

									Str_Reg[n] = Key_Reg[32];

								}else if(Str_Enc[n] == Key_Enc[66] && Str_Enc[n+1] == Key_Enc[67]){

									Str_Reg[n] = Key_Reg[33];

								}else if(Str_Enc[n] == Key_Enc[68] && Str_Enc[n+1] == Key_Enc[69]){

									Str_Reg[n] = Key_Reg[34];

								}else if(Str_Enc[n] == Key_Enc[70] && Str_Enc[n+1] == Key_Enc[71]){

									Str_Reg[n] = Key_Reg[35];

								}else if(Str_Enc[n] == Key_Enc[72] && Str_Enc[n+1] == Key_Enc[73]){

									Str_Reg[n] = Key_Reg[36];

								}else if(Str_Enc[n] == Key_Enc[74] && Str_Enc[n+1] == Key_Enc[75]){

									Str_Reg[n] = Key_Reg[37];

								}else if(Str_Enc[n] == Key_Enc[76] && Str_Enc[n+1] == Key_Enc[77]){

									Str_Reg[n] = Key_Reg[38];

								}else if(Str_Enc[n] == Key_Enc[78] && Str_Enc[n+1] == Key_Enc[79]){

									Str_Reg[n] = Key_Reg[39];

								}else if(Str_Enc[n] == Key_Enc[80] && Str_Enc[n+1] == Key_Enc[81]){

									Str_Reg[n] = Key_Reg[40];

								}else if(Str_Enc[n] == Key_Enc[82] && Str_Enc[n+1] == Key_Enc[83]){

									Str_Reg[n] = Key_Reg[41];

								}else if(Str_Enc[n] == Key_Enc[84] && Str_Enc[n+1] == Key_Enc[85]){

									Str_Reg[n] = Key_Reg[42];

								}else if(Str_Enc[n] == Key_Enc[86] && Str_Enc[n+1] == Key_Enc[87]){

									Str_Reg[n] = Key_Reg[43];

								}else if(Str_Enc[n] == Key_Enc[88] && Str_Enc[n+1] == Key_Enc[89]){

									Str_Reg[n] = Key_Reg[44];

								}else if(Str_Enc[n] == Key_Enc[90] && Str_Enc[n+1] == Key_Enc[91]){

									Str_Reg[n] = Key_Reg[45];

								}else if(Str_Enc[n] == Key_Enc[92] && Str_Enc[n+1] == Key_Enc[93]){

									Str_Reg[n] = Key_Reg[46];

								}else if(Str_Enc[n] == Key_Enc[94] && Str_Enc[n+1] == Key_Enc[95]){

									Str_Reg[n] = Key_Reg[47];

								}else if(Str_Enc[n] == Key_Enc[96] && Str_Enc[n+1] == Key_Enc[97]){

									Str_Reg[n] = Key_Reg[48];

								}else if(Str_Enc[n] == Key_Enc[98] && Str_Enc[n+1] == Key_Enc[99]){

									Str_Reg[n] = Key_Reg[49];

								}else if(Str_Enc[n] == Key_Enc[100] && Str_Enc[n+1] == Key_Enc[101]){

									Str_Reg[n] = Key_Reg[50];

								}else if(Str_Enc[n] == Key_Enc[102] && Str_Enc[n+1] == Key_Enc[103]){

									Str_Reg[n] = Key_Reg[51];

								}else if(Str_Enc[n] == Key_Enc[104] && Str_Enc[n+1] == Key_Enc[105]){

									Str_Reg[n] = Key_Reg[52];

								}else if(Str_Enc[n] == Key_Enc[106] && Str_Enc[n+1] == Key_Enc[107]){

									Str_Reg[n] = Key_Reg[53];

								}else if(Str_Enc[n] == Key_Enc[108] && Str_Enc[n+1] == Key_Enc[109]){

									Str_Reg[n] = Key_Reg[54];

								}else if(Str_Enc[n] == Key_Enc[110] && Str_Enc[n+1] == Key_Enc[111]){

									Str_Reg[n] = Key_Reg[55];

								}else if(Str_Enc[n] == Key_Enc[112] && Str_Enc[n+1] == Key_Enc[113]){

									Str_Reg[n] = Key_Reg[56];

								}else if(Str_Enc[n] == Key_Enc[114] && Str_Enc[n+1] == Key_Enc[115]){

									Str_Reg[n] = Key_Reg[57];

								}else if(Str_Enc[n] == Key_Enc[116] && Str_Enc[n+1] == Key_Enc[117]){

									Str_Reg[n] = Key_Reg[58];

								}else if(Str_Enc[n] == Key_Enc[118] && Str_Enc[n+1] == Key_Enc[119]){

									Str_Reg[n] = Key_Reg[59];

								}else if(Str_Enc[n] == Key_Enc[120] && Str_Enc[n+1] == Key_Enc[121]){

									Str_Reg[n] = Key_Reg[60];

								}else if(Str_Enc[n] == Key_Enc[122] && Str_Enc[n+1] == Key_Enc[123]){

									Str_Reg[n] = Key_Reg[61];

								}else if(Str_Enc[n] == Key_Enc[124] && Str_Enc[n+1] == Key_Enc[125]){

									Str_Reg[n] = Key_Reg[62];

								}else if(Str_Enc[n] == Key_Enc[126] && Str_Enc[n+1] == Key_Enc[127]){

									Str_Reg[n] = Key_Reg[63];

								}

						n = n+2;

					}

					printf("\n");
					printf("-----------");
					printf("\n-DECRYPTED-");
					printf("\n-----------");
					printf("\n\n");

					for(n=0;n!=Strlen_Enc;n++){
						printf("%c",Str_Reg[n]);
						Str_Reg[n]=Ept[n];
						Str_Enc[n]=Ept[n];
						Str_Enc[n+1]=Ept[n+1];
						n++;
					}

					scanf("%c",&v);

			}else{

				system("cls");
				printf("[INVALID CHOICE]");
				getch();
				system("cls");

			}

		}else if(Opt == 3){

			Con = Opt - 1;
			do{
						system("cls");
						printf("\nAre you sure?\n");
						printf("[1] Return to main menu.\n[2] Quit.\n");
						scanf("%d",&Con);
						system("cls");
					}while(Con > 2);

		}else if(Opt > 3){

			printf("[INVALID CHOICE]\n");
			getch();

		}


	}while(Con != 2);

	return 0;
}