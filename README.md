# _printf
```_printf``` is a custom implementation of the C programming function ```printf```.

**Prototype:** ```int _printf(const char *, ...);```

## Some Examples
**Integer**
* Input: ```_printf("There are %i cartons of milks at home\n", 12);```
* Output: ```There are 12 cartons of milks at homes```

**Character**
* Input: ```_printf("The first letter in the alphabet is %c\n", 'A');```
* Output: ```The first letter in the alphabet is A```

**String**
* Input: ```_printf("%s\n", 'This is a string.');```
* Output: ```This is a string.```

**Decimal:**
* Input: ```_printf("%d\n", 1000);```
* Output:  ```1000```

**Rot13**
* Input: ```_printf("Unknown:[%R]\n", "HELLO WORLD");```
* Output:  ```URYYB JBEYQ```

**FLAGS**
* Input: ```printf("Flag: [%+ d]", 1230);```
* Output:  ```Flag: [+1230] => 13```

**OCTAL**
* Input: ```printf("Unsigned octal:[%o]", 6);```
* Output:  ```Unsigned octal:[6] => 18```

Authors: 
 <h1 style="position: absolute; color: red; bottom: 15px; transform: translate(-50%, 0); left: 50%"> AUTHORS</h1>


<p align="center">

  <img src="https://readme-typing-svg.herokuapp.com?color=C94471&lines=joy+onuh+%7C%7C+and+%7C%7C+mordecai+Etukudo+aka+martcpp;contributed+%7C%7C+alot+%7C%7C+to+%7C%7C+the+Project;Hope+you+like+it;Never+Stop+Learning!&center=true&width=800&height=45" alt="martcpp">

</p>











## Project Requirements
* All files will be compiled on Ubuntu 20.04 LTS
* Programs and functions will be compiled with gcc 9.5.4 using flags -Wall -Werror -Wextra and -pedantic
* Code must follow the [Betty] style
* Global variables are not allowed
* Authorized functions and macros:
  * ```write``` (man 2 write)
  * ```malloc``` (man 3 malloc)
  * ```free``` (man 3 free)
  * ```va_start``` (man 3 va_start)
  * ```va_end``` (man 3 va_end)
  * ```va_copy``` (man 3 va_copy)
  * ```va_arg``` (man 3 va_arg)

## Mandatory Tasks
- [x] Write function that produces output with conversion specifiers ```c```, ```s```, and ```%```.
- [x] Handle conversion specifiers ```d```, ```i```.
- [x] Create a man page for your function.
## Advanced Tasks
- [x] Handle conversion specifier ```b```.
- [x] Handle conversion specifiers ```u```, ```o```, ```x```, ```X```.
- [x] Use a local buffer of 1024 chars in order to call write as little as possible.
- [x] Handle conversion specifier ```S```.
- [x] Handle conversion specifier ```p```.
- [x] Handle flag characters ```+```, space, and ```#``` for non-custom conversion specifiers.
- [ ] Handle length modifiers ```l``` and ```h``` for non-custom conversion specifiers.
- [ ] Handle the field width for non-custom conversion specifiers.
- [ ] Handle the precision for non-custom conversion specifiers.
- [ ] Handle the ```0``` flag character for non-custom conversion specifiers.
- [x] Handle the custom conversion specifier ```r``` that prints the reversed string.
- [x] Handle the custom conversion specifier ```R``` that prints the rot13'ed string.
- [ ] All above options should work well together.
## File Descriptions
-**_printf.c**
* contains the  fucntion ```_printf```, which uses the prototype ```int _printf(const char *format, ...);```. The format string is composed of zero or more directives. See ```man 3 printf``` for more detail. **_printf** will return the number of characters printed (excluding the null byte used to end output to strings) and will write output to **stdout**, the standard output stream.


**main.h**
*contains all function prototypes used for ```_printf```.

**man_3_printf**
* manual page for the custom ```_printf``` function.

**print_char.c** **print_int.c** **pointer.c**
* contains all function of each specifier used for ```_printf```.
* all function have its own description inside the file.

**formatter.c**
* contains arguments types used for ```_printf```.

**flags.c**
* contains all function for each flag use for ```_printf```.

**utils.c**
* contains some necessary functionalities for ```_printf```.

**width.c**
* contains functions to get width for spcifics spcifiers.

**write.c**
* contains write functions.
