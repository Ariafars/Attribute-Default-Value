# Attribute-Default-Value
#include <cmath>
 3 using namespace std;
 4 struct point{
 5   double x, y;
 6   void input(void) {
 7     cout << "Enter X: ";
 8     cin >> x;
 9     cout << "Enter Y: ";
10     cin >> y;
11   }
12   void print(void) {
13     cout << '(' << x << ','
14       << y << ')' << endl;
15   }
16   void move(double dx=1, double dy=0){
17     x += dx;
18     y += dy;
19   }
20   double magnitude(void){ // length
21     return sqrt(pow(x, 2)+pow(y, 2));
22   }
23 };
24 int main(){
25   point p1;
26   p1.print();
27   p1.input();
28   p1.print();
29   p1.move(3);
30   cout << p1.magnitude() << endl;
31 }
