Victor Kalevich
========================
Contacts
------------------------
+ [VK](https://vk.com/nativehero)
+ [Instagram](https://www.instagram.com/ddmnnhll/)
+ [YouTube](https://www.youtube.com/channel/UCI4jsGg7p3DFbTWA48hFp6w)
+ [Facebook](https://www.facebook.com/profile.php?id=100010316671092)

Some info about me
------------------------
My main goal is to succeed in the field of programming. My main qualities are perseverance and hard work. I easily remember and assimilate new information, as well as cope with tasks. Unfortunately, I have no work experience, but I really want to get a job in the company.

My skills
------------------------
+ C++
+ C#
+ HTML
+ CSS
+ JS(some)
+ Visual Studio
+ VS Code
+ Unity
+ Notepad++

Code example
------------------------
`C++`

```
template <typename no, typename person> class bank
{
	no* number;
	person* cc;
public:
	bank(no number[], person cc[]);

	void print()
	{
		cout << "NAME OF THE BANK VISITORS: " << endl;
		for (int i = 0; i < n; i++)
		{
			for (int j = 0; j < n; j++)
			{
				cout << " " << cc[i][j];
			}
		}
		cout << endl;
	}
	void print2()
	{
		cout << "NAME OF SCORES: " << endl;
		for (int i = 0; i < 5; i++)
		{
			cout << " " << number[i];
		}
	}
};
template <typename no, typename person> bank<no, person>::bank(no score[], person mas[])
{
	int len1 = sizeof(score) + 1;
	number = new no[len1];
	long len = sizeof(mas) + 1;
	cc = new person[len];
	delete[] cc;
	long len2 = sizeof(mas) + 1;
	cc = new person[len2];
	for (int i = 0; i < len2; i++)
	{
		cc[i] = mas[i];
	}

	for (int cout = 0; cout < len1; cout++)
	{
		cc[cout] = mas[cout];
	}
	for (int got = 0; got < len; got++)
	{
		number[got] = score[got];
	}
}

int main()
{
	string score[5];
	int n;
	cin >> n;
	char mas[n][20];
	char temp;
	cout << "Enter the users name: " << endl;
	for (int i = 0; i < n; i++)
	{
		for (int j = 0; j < n; j++)
		{
			cin >> mas[i][j];
		}
	}
	for (int i = 0; i < n; i++)
	{
		for (int j = 0; j < n - i - 1; j++)
		{
			if (strcmp(&mas[j], &mas[j + 1]) > 0)
			{
				temp = mas[j];
				mas[j] = mas[j + 1];
				mas[j + 1] = temp;
			}
		}
	}
	for (int i = 0; i < n; i++) {
		cout << mas[i] << endl;
	}
	cout << "Enter the scores: " << endl;
	for (int i = 0; i < 5; i++)
	{
		cin >> score[i];
	}
	bank<string, char> page(score, mas);
	page.print();
	page.print2();
}
```

Work experience
------------------------
I have no work experience.
I completed courses in C++ and C# from the Center for Learning Technologies

Education
------------------------
At the moment, I have completed two courses at the University of Informatics and Radio Electronics, majoring in medical electronics

English
------------------------
I speak good English. I can express my thoughts freely, and I also have a good command of technical English.
