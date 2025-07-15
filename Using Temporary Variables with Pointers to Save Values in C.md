# Using Temporary Variables with Pointers to Save Values in C

When working with pointers in C, it's common to encounter situations where you need to modify multiple values from a function. But what if those values depend on each other, and changing one too early would overwrite important information?
That’s where **temporary variables** come in. Temporary variables are used to **store intermediate values**, so you don’t lose important data during computation.

## Example: Division and Modulo with Pointers
`#include <stdio.h>

void	ft_ultimate_div_mod(int *a, int *b)
{
	int	tdiv;
	int	tmod;

	tdiv = *a / *b;
	tmod = *a % *b;
	*a = tdiv;
	*b = tmod;
}

int main(void)
{
	int x = 96;
	int y = 42;

	printf("BEFORE change %d %d | address: %p %p\n", x, y, &x, &y);
	ft_ultimate_div_mod(&x, &y);
	printf("AFTER change %d %d | address: %p %p\n", x, y, &x, &y);
	return(0);
}



