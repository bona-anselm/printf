The `printf` project is our first __collabarative__ project at the ALX SE program. 
We are to create a `_printf` function which immitates the actual `C` `printf` function by printing in formated output. 
So we are to consider different **character specifiers** among other things. 
The project pretty much requires us to use all of the concept we have learned in the program so far to implement it.

_printf() is a function that performs formatted output conversion and prints data. It has the following  prototype:

	```int _printf(const char *format, ...)```

Where `format` contains the string that is printed. As `_printf()` is a variadic function, it can receives `n` number of arguments that's replaced by n tags written inside the string.

The format tags prototype is the following:

	```%[flags][length]specifier```
	
If the program runs successfully, the *return value* is the amount of characters printed.
	
| Specifier | Output |
| ------------- | ------------- |
| c  | Character  |
| d or i | Signed decimal integer |
| s  | String of characters  |
| b  | Signed binary  |
| o  | Signed octal  |
| u  | Unsigned integer  |
| x  | Unsigned hexadecimal  |
| X  | Unsigned hexadecimal (uppercase)  |
| p  | Pointer address  |
| r  | Reverse string of characters |
| R  | ROT13 translation of string |
| S  | String with special chars replaced by their ASCII value  |
| %  | Character  |

| Flags | Description | Specifiers |
| ------------- | ------------- | ------------- | 
| +  | Prints a plus sign (+) when the argument is a positive number. In other case, prints a minus sign (-). | i, d |
| (space) | Prints a blank space if the argument is a positive number | i, d |
| #  | Prints 0, 0x and 0X for o, x and X specifiers, respectively. It doesn't print anything if the argument is zero | o, x, X |

| Length | Description | Specifiers |
| ------------- | ------------- | ------------- | 
| l | Prints a long int or unsigned long int | i, d, o, u, x and X |
| h | Prints a short int or unsigned short int | i, d, o, u, x and X |



|FILES			|FUNCTIONS							|
|-----------------------|---------------------------------------------------------------|
|**main.h**		|Header file containing all funtion prototypes and libraries	|
|**_printf.c**		|Produces output according to a formated			|
|**get_func.c**	|Function pointer that selects the right function for each Operation.	|
|**print_buf.c**|Print ths buffer							|
|**handl_buf.c**|Concatenates buffer characters						|
|**print_chr.c**|Writes character to stdout ```identifier: %c```			|
|**print_str.c**|Writes strings to stdout ```identifier: %s```				|
|**print_int.c**|Writes integer to stdout ``identifier: %i``` or `%d`			|
|**print_bnr.c**|Prints decimal in binary ```identifier: %b```				|
|**print_oct.c**|Prints decimal to octal ```identifier: %o```				|
|**print_hex.c**|Prints decimal to hexadecimal ```identifier: %x```			|
|**print_upx.c**|Prints decimal to uppercase hexadecimal ```identifier: %X```		|
|**print_usr.c**|Prints a string and values of non-printed chars ```identifier: %S```	|
|**print_unt.c**|Prints an unsigned integer ```identifier: %u```			|
|**print_rev.c**|Prints strings to stdout in reverse ```identifier: %r```		|
|**print_rot.c**|Prints strings to stdout in rot13 ```identifier: %R```			|
|**print_add.c**|Prints the address of an input variable ```identifier: %p```		|
|**print_long_oct.c**|Prints long decimal number to octal ```identifier: %lo```		|
|**print_long_hex.c**|Prints long decimal number to hexadecimal ```identifier: %lx```	|
|**print_long_int.c**|Prints long integer ```identifier: %li```				|
|**print_long_upx.c**|Prints long decimal in uppercase hexadecimal ```identifier: %lX	|
|**print_long_unt.c**|Prints a long unsigned integer ```identifier: %lu```		|
|**print_short_oct.c**|Prints short decimal number to octal ```identifier: %ho```	|
|**print_short_hex.c**|Prints short decimal number in hexadecimal ```identifier: %hx```	|
|**print_short_int.c**|Prints a short integer ```identifier: %hi```			|
|**print_short_upx.c**|Prints a short decimal to uppercase hexadecimal ```identifier: %hX```||**print_short_unt.c**|Prints a short unsigned integer ```identifier: %hu```		|
|**print_num_hex.c**|Print a number in hexadecimal begining with 0 And x ```identifier: %#x```|
|**print_num_oct.c**|Prints a number in octal begining with 0 and o ```identifier: %#o```|
|**print_num_upx.c**|Prints a number in uppercase hexadecimal ```identifier: %#X```|
|**print_plus_int.c**|Prints an integer with plus symbol ```identifier: %+i```	|
|**print_space_int.c**|Prints an integer beginning with 0 and u ```identifier: % i```	|
|**print_func_ids.c**|Returns the number of identifiers		|



