





#include<iostream>
#include<string>
using namespace std;

class Person {
	string name, hobby;
	int age;
	int score;
public:
	Person() {};
	Person(string n, string h, int a) : name(n), hobby(h), age(a) {};
	void Show()
	{cout << "이름 : " << name << "  나이 : " << age << "  취미 : " << hobby << endl;}
	void Study() { cout << "공부에 집중하기" << endl; }
	void Rest() { cout << "휴식하기 " << endl; }
};
int main()
{
	Person Shin("신은지", "게임하기", 21);

	Shin.Show();

	for (int i = 0; i < 10; i++) {
		Shin.Study();
		if (i == 5) break;
	}
	Shin.Rest();
}
