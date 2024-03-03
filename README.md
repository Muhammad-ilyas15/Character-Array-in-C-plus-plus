
//                                                                  CHARACTER ARRAYS
//                                                                   ---------------
//                                                                   ---------------

//                              Q_Find length, words, lines of character array
/*
int strLength(char ch[]) {
	int i = 0,count=0;
	while (ch[i++] != '\0') {
		if (ch[i] == ' ' || ch[i] == '\n')
			continue;
		count++;
	}
	
	return count;
}
int strWords(char ch[]) {
	int i = 0, count = 0;
	while (ch[i++] != '\0') {
		// abc__\n\n__how are you\0 OR \n how are you$
		if ((ch[i] == ' ' || ch[i + 1] == '\0' || ch[i] == '\n') && (ch[i - 1] != ' ' && ch[i - 1] != '\n'))
			count ++;
	}
	return count;
}
int strLines(char ch[]) {
	int i = 0, count = 0;
	while (ch[i++] != '\0') {
		if (ch[i] == '\n' && ch[i - 1] != '\n' || ch[i + 1] == '\0' )
			count++;
	}
	return count;
}
int main() {
	char name[100];
	cin.getline(name, 100, '$');
	cout << "Number of characters in array is " << strLength(name) << endl;
	cout << "Number of words in array is "<<strWords(name) << endl;
	cout << "Number of line in array is " << strLines(name) << endl;
}
*/

//                                                Q-Reverse character array
/*
int sizeArray(char ch[]) {
	int i = 1;
	while (ch[i++] != '\0');
	return i-1;
}


void reverseArray(char ch[]) {
	int size = sizeArray(ch);
	cout << "size of array is " << size << endl;
	int i = -1;
	char chr;
	while (i++ <= size / 2)// condition check on i previous value and when entering into body of loop it will use incremented value of i

	{
		chr = ch[i];
		ch[i] = ch[size - i-1];
		ch[size - i-1] = chr;
		i++;
	}
}
int main() {
	char ch[100];
	cin >> ch;
	reverseArray(ch);
	cout << "Reversed Array is " << ch;
}
*/
//                                               Q. Palindrome check.  
/*

bool checkPalindrome(char ch[], int size) {
	int i = 0;
	while (i <= size / 2) {
		if (ch[i] != ch[size - i - 1])
			return false;
		i++;
	}
	return true;
}
int main() {
	char ch[100];
	cin >> ch;
	int i = 1;
	while (ch[i++] != '\0');
	int size = i - 1;
	bool flag=checkPalindrome(ch, size);
	if (flag == true)
		cout << "entered array is palindrome" << endl;
	else
		cout << "entered array is not palindrome" << endl;

}
*/
