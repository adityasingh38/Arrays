
# Arrays

Arrays in C are a collection of variables of the same type that are accessed using an index. An array is declared by specifying the data type of the elements in the array, followed by the name of the array, and then the size of the array in square brackets.

![Arrays-in-C](https://user-images.githubusercontent.com/88421625/234410125-1baa80ed-d156-458d-be86-be154fc04067.png)


Here is an example of declaring an integer array with 5 elements:
```
int myArray[5];
```
This declares an array called 'myArray' that can hold 5 integers. The first element of the array is 'myArray[0]', the second is 'myArray[1]', and so on.

You can also initialize an array at the time of declaration, like this:
```
int myArray[5] = {1, 2, 3, 4, 5};
```
In this case, the array is initialized with the values 1, 2, 3, 4, and 5.

You can access individual elements of an array using their index. For example, to access the third element of 'myArray', you would use the following:
```
int thirdElement = myArray[2];
```
Arrays in C are zero-indexed, meaning that the first element of an array has an index of 0. So the second element of 'myArray' would have an index of 1, and so on.
## Key Points
Here are some important points about Arrays:

- Arrays are declared by specifying the data type of the elements in the array, followed by the name of the array, and then the size of the array in square brackets.
- Arrays in C are zero-indexed, meaning that the first element of an array has an index of 0.
- You can initialize an array at the time of declaration, or you can initialize individual elements of the array later.
- You can access individual elements of an array using their index. You can also use loops to access and manipulate the elements of an array.
- Arrays in C are not dynamically resizable, meaning that you cannot change the size of an array once it has been declared.
- Arrays in C are passed to functions by reference, meaning that any changes made to the array inside the function will affect the original array.
- Arrays can be used for a wide range of purposes, from storing a collection of numbers to representing strings and more complex data structures.







# Code

```bash
#include <stdio.h>

int main()
{
	int i, j;
	int x[5] = {2, 15, 16, 22, 29};
	
	
	// 3. storing and printing a string, which is essentially a character array, and then printing array elements at even indexes:
	
	char name[] = "PROGRAMMING";
	printf("Value stored in the string (character array): %s \n\n", name);
	
	printf("String characters at even indexes: \n");
	
	for(j = 0; j < sizeof(name); j++)
	{
		if(j % 2 == 0)
		{
			printf("%c", name[j]);
		}
		else
		{
			printf("\n");
		}
	}
	
	
	
	
	// 2. Taking an array index as input from the user and printing the element at that index in that array:
	
	//int user_index;
	
	//printf("Enter index: ");
	//scanf("%d", &user_index);
	
	//if((user_index < 0) || (user_index >= 4))
	//{
	//	  printf("invalid index \n\n");
	//}
	//else
	//{
	//    printf("Element at array index %d: %d \n\n", user_index, x[user_index]);
	//}
	
	
	
	
	// 1. Printing the first array element along with the rest of the array using a for loop:
	
	//printf("First array element: %d \n\n", x[0]);
	
	//for(i = 0; i < 5; i++)
	//{
	//    printf("Array element %d: %d", i, x[i]);
	//	  printf("\n");
	//}
	
	
	return 0;
}
```
## Output
![Screenshot 2023-04-26 030337](https://user-images.githubusercontent.com/88421625/234409934-3b56f26c-5f7d-43f7-b355-a998305e510f.png)

![Screenshot 2023-04-26 030514](https://user-images.githubusercontent.com/88421625/234409857-e2200eeb-5eb6-4222-b9b6-2f53bc51197d.png)

![Screenshot 2023-04-26 030622](https://user-images.githubusercontent.com/88421625/234409880-0bbbb466-1e4d-406a-8c09-1585eee7ef64.png)

![Screenshot 2023-04-26 030700](https://user-images.githubusercontent.com/88421625/234409955-5657aab7-3ffc-43ef-b3c6-7ad58ef09e4f.png)
