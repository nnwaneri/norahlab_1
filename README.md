# norahlab_1
This is the bubble sort for lab 1.
#include <iostream>
#include <vector>
#include <string>
using namespace std;
void bubbleSort(vector<int> &a) {
	for (int i = 1; i < a.size(); i++) {
		for (int k = 0; k < a.size() - 1; k++) {
			if (a[k] > a[i]) swap(a[k], a[i]);
		}
	}
}
int main() {
	vector<int> a = { 34, 12, 1, 20, 4, 6, 78 };
	bubbleSort(a);
	for (int i = 0; i < a.size(); i++) {
		cout << a[i] << '\n';
	}
	system("pause");
	return 0;
}
/*
1
4
6
12
20
34
78
*/

int main() {
	string myArray[5];
	int i, j, num;
	cout << "\nHow many times would you like to sort?: ";
	cin >> num;
	for (i = 0; i <= 4; i++) {
		cout << "\nEnter the name: ";
		cin >> myArray[i];
	}
	for (i = 0; i <= 3; i++) {
		for (j = i + 1; j <= 5; j++) {
			string temp;
			if (myArray[i] > myArray[j]) {
				temp = myArray[i];
				myArray[i] = myArray[j];
				myArray[j] = temp;
			}
		}
	}
	for (i = 0; i <= 4; i++) {
		cout << '\n' << myArray << '\n';
	}
	system("pause");
	return 0;
}
/*
How many times would you like to sort?: 5

Enter the name: mango

Enter the name: apple

Enter the name: strawberry

Enter the name: pear

Enter the name: kiwi

apple

kiwi

mango

pear

strawberry
*/

