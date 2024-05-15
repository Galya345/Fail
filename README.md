# Fail
#include <iostream>
#include <string>

using namespace std;
struct LunchBite
{
	bool ork : 1;
	bool second : 1;
	bool drink : 1;
	bool salad : 1;
};
struct Lunch
{
	bool ork1 : 1;
	bool second1 : 1;
	bool drink1 : 1;
	bool salad1 : 1;
};
struct SoupBite
{
	short var : 2;
	bool top : 2;
};
void checkMeal(LunchBite p);
void checkMeal(Lunch p);
int main()
{
	setlocale(LC_ALL, "ru");
	
	int a;
	
	cout << "Выберите класс \n";
	cout << "Орк-1, Эльф, Человек, Гном \n";
	cin >> a;

	cout << sizeof(LunchBite) << endl;
	LunchBite p1;
	p1.ork = 1;
	p1.second = 0;
	p1.salad = 0;
	p1.drink = 1;
	cout << sizeof(p1) << endl;
	checkMeal(p1);

	cout << sizeof(Lunch) << endl;
	Lunch p2;
	p2.ork1 = 1;
	p2.second1 = 0;
	p2.salad1 = 0;
	p2.drink1 = 1;
	cout << sizeof(p1) << endl;
	checkMeal(p1);
	return 0;
}
void checkMeal(LunchBite p)
{
	if (p.ork)
	{
		cout << "Орк." << endl;
		SoupBite s;
		short soup;
		cout << "Выберите орка: 1-шаман, 2-копейшик, 3-гоблин\n";
		cin >> soup;
		s.var = soup;
		if (s.var == 1)
			cout << "Будет шаман." << endl;
		else if (s.var == 2)
			cout << "Будет копейшик." << endl;
		else if (s.var == 3)
			cout << "Будет гоблин." << endl;
	}
	if (p.second)
	{
		cout << "Эльф." << endl;
		SoupBite s;
		short second;
		cout << "Выберите эльфа: 1-магистр, 2-лучник, 3-воин\n";
		cin >> second;
		s.var = second;
		if (s.var == 1)
			cout << "Будет магистр." << endl;
		else if (s.var == 2)
			cout << "Будет лучник." << endl;
		else if (s.var == 3)
			cout << "Будет воин." << endl;
	}
	if (p.salad)
	{
		cout << "Человек." << endl;
		SoupBite s;
		short salad;
		cout << "Выберите человек: 1-стрелец, 2-рыцарь, 3-маг\n";
		cin >> salad;
		s.var = salad;
		if (s.var == 1)
			cout << "Будет стрелец." << endl;
		else if (s.var == 2)
			cout << "Будет рыцарь." << endl;
		else if (s.var == 3)
			cout << "Будет маг." << endl;
	}
	if (p.drink)
	{
		cout << "Гном." << endl;
		SoupBite s;
		short drink;
		cout << "Выберите гнома: 1-кузнец, 2-молотобоец, 3-друг\n";
		cin >> drink;
		s.var = drink;
		if (s.var == 1)
			cout << "Будет кузнец." << endl;
		else if (s.var == 2)
			cout << "Будет молотобоец." << endl;
		else if (s.var == 3)
			cout << "Будет друг." << endl;
	}
	


}
void checkMeal(Lunch p)
{
	if (p.ork1)
	{
		cout << "Орк." << endl;
		SoupBite s;
		short soup;
		cout << "Выберите орка: 1-шаман, 2-копейшик, 3-гоблин\n";
		cin >> soup;
		s.var = soup;
		if (s.var == 1)
			cout << "Будет шаман." << endl;
		else if (s.var == 2)
			cout << "Будет копейшик." << endl;
		else if (s.var == 3)
			cout << "Будет гоблин." << endl;
	}
	if (p.second1)
	{
		cout << "Эльф." << endl;
		SoupBite s;
		short second;
		cout << "Выберите эльфа: 1-магистр, 2-лучник, 3-воин\n";
		cin >> second;
		s.var = second;
		if (s.var == 1)
			cout << "Будет магистр." << endl;
		else if (s.var == 2)
			cout << "Будет лучник." << endl;
		else if (s.var == 3)
			cout << "Будет воин." << endl;
	}
	if (p.salad1)
	{
		cout << "Человек." << endl;
		SoupBite s;
		short salad;
		cout << "Выберите человек: 1-стрелец, 2-рыцарь, 3-маг\n";
		cin >> salad;
		s.var = salad;
		if (s.var == 1)
			cout << "Будет стрелец." << endl;
		else if (s.var == 2)
			cout << "Будет рыцарь." << endl;
		else if (s.var == 3)
			cout << "Будет маг." << endl;
	}
	if (p.drink1)
	{
		cout << "Гном." << endl;
		SoupBite s;
		short drink;
		cout << "Выберите гнома: 1-кузнец, 2-молотобоец, 3-друг\n";
		cin >> drink;
		s.var = drink;
		if (s.var == 1)
			cout << "Будет кузнец." << endl;
		else if (s.var == 2)
			cout << "Будет молотобоец." << endl;
		else if (s.var == 3)
			cout << "Будет друг." << endl;
	}



}
