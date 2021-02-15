# optional-2
#include <iostream>
using namespace std;
int main() {
const int MIN_YEARS = 1;
const int MIN_RAIN = 0;
int years;
double rainfall;
double totalRainfall = 0;

cout << "How many years has there been rainfall?" << endl;
do {
  cout << "the number could not be less than " << MIN_YEARS << endl;
  cout << "number of years: " << endl;
  cin >> years;
}
while (years < MIN_YEARS);

for (int year = 1; year <= years; year++) {

  for (int quater = 1; quater <= 4; quater++) {
    cout << "Please enter the inches for the quater" << endl;
    do {
      cout << "the number cannot be less than " << MIN_RAIN;
      cout << "Inches of rainfall: " << endl;
      cin >> rainfall;
    }
  while (rainfall < MIN_RAIN);

  totalRainfall += rainfall;
  }
}
cout << "Total number of months: " << (years * 12) << endl;
cout << "Total inches of rainfall: " << totalRainfall << endl;
cout << " Average monthly rain: " << totalRainfall/(years*12) << endl;

}
