#include <iostream>

void main()
{
	setlocale(LC_ALL, "ru");

	//exercise 1 
	const int columns = 5, lines = 5;
	int arr[lines][columns];
	int num{};
	int counter = 1;

	std::cout<<"Нужно будет ввести любое число для того чтобы заполнить двумерный массив" << std::endl;
	std::cout << "Введите любое число: ";
	std::cin >> num;

	for (int i = 0; i < lines; i++)
	{
		for (int j = 0; j < columns; j++) 
		{
			arr[i][j] = num * counter;
			std::cout << arr[i][j] << " ";
			counter *= 2;
		}
		std::cout << "\n";
	}



	std::cout << "\n\n\n";

	// exercise 2
	const int col = 5, ln = 5;
	int arr2[ln][col];
	int inputNum;
	int counterr = 0;

	std::cout << "Введите любое число: ";
	std::cin >> inputNum;

	for (int i = 0; i < col; i++)
	{
		for (int j = 0; j < ln; j++)
		{
			arr[i][j] = inputNum + counterr;
			counterr += 1;
			std::cout << arr[i][j] << " ";
		}
		std::cout << "\n";
	}
}
