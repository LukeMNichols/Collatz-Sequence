# Collatz-Sequence
Simple C++ program that produces the Collatz sequence from a starting number(n)

#include <iostream>
#include <cmath>
#include <random>
#include <vector>

using namespace std;

int main() {
	int i;
	int j;
	int n;
	int x;
	cout << "What is the intial number?" << "\n";
	cin >> x;
	int temp = x;
	while (temp != 1) {
		if ((temp % 2) == 0) {
			temp = (temp) / 2;
		}
		else {
			temp = 3*(temp)+1;
		}
		cout << temp << ",";
	}
}
