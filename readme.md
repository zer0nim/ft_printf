# 42 _ ft_printf

Are you not allowed to use printf?

**You can recode yours 😉!** It will be a chance for you to discover a feature of the C language – variadic
functions – and to practice detailed management of the printing options.

## Compiling
> Made for OS X only

Run `Make`

## Usage
#### ft_printf functionality

* the following conversions:

  `s S p d D i o O u U x X c C b B`
* `%%`
* the flags `# 0 - +` and `space`
* minimum field-width
* precision with `.`
* size prefix `hh h l ll j z`

#### Example
```
// include the header in your project
#include "ft_printf.h"

int	main(void)
{
	int arr[] = {98, 360, -2, 51};

	for (int i = 0 ; i < 4 ; ++i)
		ft_printf("arr[%d] = %+4d\n", i, arr[i]);

	return (0);
}
```
`$> gcc main.c libftprintf.a`

`$> ./a.out`
```
arr[0] =  +98
arr[1] = +360
arr[2] =   -2
arr[3] =  +51
```
