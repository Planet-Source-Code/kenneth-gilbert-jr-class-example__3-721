<div align="center">

## Class Example


</div>

### Description

A basic example of setting up a class and using it. ANSI Compliant
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Kenneth Gilbert Jr\.](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/kenneth-gilbert-jr.md)
**Level**          |Beginner
**User Rating**    |3.6 (36 globes from 10 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Classes/ Frameworks/ OOP](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/classes-frameworks-oop__3-31.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/kenneth-gilbert-jr-class-example__3-721/archive/master.zip)





### Source Code

```
#include <iostream.h>
class Person
{
	public:
		void SetAge(int Age); // Set the age
		void SetName(char* chrName); // Set the name
		char* GetName(); // get the name
		int GetAge(); // get the age
		void Greeting1();// Say "Hello!"
		void SayName(); // Say "My name is <My Name>"
		void Goodbye(); // Say "Good bye!
		void SayAge(); // Say " I am <X> years old!"
	private:
		char* pName;
		unsigned int pAge;
};
void Person::SetAge(int Age)
{
	pAge = Age;
}
void Person::SetName(char* chrName)
{
	pName = chrName;
}
char* Person::GetName()
{
	return pName;
}
int Person::GetAge()
{
	return pAge;
}
void Person::Greeting1()
{
	cout << "Hello!\n";
}
void Person::SayAge()
{
	// Check Person age
	if (pAge < 2)
			// Person is 1 or less years old
			cout << "I am a baby!\n";
	else
			// Person is over 1 years old
			cout << "I am " << pAge << " years old!\n";
}
void Person::SayName()
{
	cout << "My name is " << pName << "!\n";
}
void Person::Goodbye()
{
	cout << "Good-bye!!\n";
}
int main()
{
	// Define our perosn
	Person Gabe;
	// Set up Gabe's age
	Gabe.SetAge(13);
	// Give Gabe's full name
	Gabe.SetName("Gabriel Halland");
	// Make Gabe greet the user
	Gabe.Greeting1();
	// Make Gabe introduce himself
	Gabe.SayName();
	// Make Gabe tell us how old he is
	Gabe.SayAge();
	// Make Gabe dismiss himself
	Gabe.Goodbye();
	// end out
	return 0;
}
```

