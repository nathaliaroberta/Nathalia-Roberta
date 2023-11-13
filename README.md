// Exercicio 1

#include <iostream>

using namespace std;

int dobro(int N){
	int d;
	d = N*2;
	return d;
}

int main()
{
 int a;
 cin >> a;
cout <<dobro(a);

return 0;       
}



//Exercicio 2

#include <iostream>
#include <stdio.h>
using namespace std;

void extenso(int dia ,int mes, int ano ){
	if(dia < 1 or dia > 31){
		cout << "Data invalida";
		return;
	}
	if(mes < 1 or mes > 12){
		cout << "Data invalida";
		return;
	}
	if(ano < 1 or ano > 9999){
		cout << "Data invalida";
		return;
	}
	
	string m[12] = {"janeiro", "fevereiro", "marco", "abril", "maio", "junho", "julho", "agosto", "setembro", "outubro", "novembro", "dezembro"};
	string s;
	char buffer[5];
	sprintf(buffer,"%2d",dia);
	s += buffer;
	s += " de ";
	s += m[mes-1];
	s += " de ";
	sprintf(buffer,"%4d",ano);
	s += buffer;
	
	cout << s;
	
}

int main()
{
	extenso(18,06,2008);
    
    return 0;       
}



 //Exercicio 3

#include <iostream>

using namespace std;

int pn (float n){
	if (n > 0){
		return 1;
	}else{
		if (n < 0){
			return -1;
		}else{
			return 0;
		}
	}
}

int main()
{
    int y;
    cin >> y;
    cout << pn(y);
    return 0;       
}


 //Exercicio 4

#include <iostream>
#include <cmath>

using namespace std;

int qp(int n){
	if(n < 0 ){
		return 0;
	}
	
	float rq = sqrt(n);	
	if(rq - int(rq) == 0){
		return 1;
	}
	
	return 0;
	
}

int main()
{
   int v;
   cin >> v;
   cout << qp(v);
    return 0;       
}




//exercicio 5

#include <iostream>
#include <cmath>

using namespace std;

float vEsfera(float R){
	float V = 4.0/3.0 * M_PI * pow(R,3);
	return V;
}

int main()
{
	int b;
	cin >> b;
    cout << vEsfera(b);
    return 0;       
}
