# Question #0
To allocate enough space for an array of 10 integers (on a 64bit, Linux machine), I can use:

[ ] malloc(64 * 10)


[ ] malloc(10 * int)


[x] malloc(10 * sizeof(int))


# Question #1
If I want to copy the string “Best School” into a new space in memory, I can use this statement to reserve enough space for it (select all valid answers):


[x] malloc(sizeof(“Best School”))


[] malloc(strlen(“Best School”))


[] malloc(11)


[x] malloc(12)


[] malloc(sizeof(“Best School”) + 1)


[x] malloc(strlen(“Best School”) + 1)


# Question #2
malloc returns a pointer


[x] True


[ ] False

# Question #3
malloc returns an address


[x] True


[] False

# Question #4
What is wrong with this code:



int cp(void)
{
    char *s;

    s = malloc(12);
    strcpy(s, "Best School");
    return (0);
}

[] You don’t have enough space to store the copy of the string “Best School”


[x] There is no comment


[] You can’t call strcpy with a string literal


[x] malloc can fail so we should check its return value all the time before using the pointers returned by the function.

# Question #5
You can do this:

free("Best School");

[] Yes


[x] No

# Question #6
You can do this:

char str[] = "Best School";

free (str);

[] Yes


[x] No

 # Question #7
You can do this:

char *s;

s = strdup("Best School");
if (s != NULL)
{
    free(s);
}

[x] Yes


[] No

# Question #8
The memory space reserved when calling malloc is on:


[] The stack


[x] The heap

# Question #9
What will you see on the terminal?

int main(void)
{
    int *ptr;

    *ptr = 98;
    printf("%d\n", *ptr);
    return (0);
}

[] 0


[] 98


[] It doesn’t compile


[x] Segmentation Fault