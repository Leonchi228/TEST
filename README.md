<<<<<<< HEAD
<<<<<<< HEAD
#include <iostream>
using namespace std;
int main() {
	int n, a, k = 0;
	cin >> n>>a;
	int* prest=new int[n];
	for (int i = 0; i < n; i++) {
		cin >> prest[i];
	}
	if (prest[a-1] == 1) k += 1;
	for (int i = a-2, j = a;;) {
		if (i >= 0 && j != n) {
			if (prest[i] == 1 && prest[j] == 1) {
				k += 2;
				i--;
				j++;
				continue;
			}
			else {
				i--;
				j++;
				continue;
			}
		}

		else if (i < 0 && j != n) {
			if (prest[j] == 1) {
				k += 1;
				j++;
				continue;
			}
			else {
				j++;
				continue;
			};
		}
		else if (i >= 0 && j == n) {
			if (prest[i] == 1) {
				k += 1;
				i--;
				continue;
			}
			else {
				i--;
				continue;
			};
		}
		if (i < 0 && j == n)break;
		
	}
	cout<< k;
}

=======
# тестовый
>>>>>>> parent of ac0408d (Update README.md)
=======
# тестовый
>>>>>>> parent of ac0408d (Update README.md)
# тест
# тестовый
