#include "stdafx.h" 
#include "iostream" #include "sstream"

using namespace std;

int main() 
{ int max1,max2, i, a1[10], a2[10];

for (string string; getline(cin, string); ) {
	          istringstream stream(string);
	              bool failure = false;
	                    for (int i = 1; i <= 10; ++i) {
		                     if (!(stream >> a1[i])) {
			                            failure=true;
			break;
		}
	}

	max1 = a1[1];

	if (!failure) {
		for (int i = 1; i <= 10; ++i) {
			if (a1[i] > max1) {
				  max1 = a[i];
			}
		}
	
		break;
	}
	else {
		cout << "An error has occured while reading numbers from line" << endl;
	}
}

for (string string; getline(cin, string); ) {
	istringstream stream(string);
	bool failure=false;
	       for (int i = 1; i <= 10; ++i) {
	            	if (!(stream >> a2[i])) {
			                failure = true;
		                      	break;
		} 
	}

	max2 = a2[1];

	   if (!failure) {
		      for (int i = 1; i <= 10; ++i) {
			     if (a2[i] > max2) {
				max2 = a2[i];
			}
		}
		
		break;
	}
	else {
		cout << "An error has occured while reading numbers from line" << endl;
	}
}

cout << max1 + max2 << endl;

system("pause");
cin.get();

return 0;
}
