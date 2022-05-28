data types

quialifiers 
  unsigned
    double positive value, but lose negative values. goes from 0 to ~4 billion (no negatives)
  short, long, const

int
  whole numbers, no decimal points
  always take up 4 bytes (32 bits) of memory; values are limited to 32 bits worth of information
  ~2 billion to the positive; 2 billion to the negative

char
  variables that will store single character. 
  always take up 1 byte (8 bit) of memory; values are limited to 8 bits worth of information
  ASCII
  A, 65
  a, 97
  0, 48
  
float
  real numbers, have decimal points
  always take up 4 bytes (32 bits) of memory; values are limited to 32 bits worth of information
  precision issues due to limited number of digits

double
  same as float but double
  always take up 8 bytes (64 bits) of memory; values are limited to 64 bits worth of information
  more precision then float; extra 32 bits to work with

void
  type, not a data type
  cannot be set as a variable, cannot assign a value to void
  functions can have void return type (dont return a value)
  int main (void)
  take no argument 
  placeholder for "nothing", no return values no parameters0

bool
  Boolean value, holding 2 distinct values
  True/False
  
string
  words, collections of characters
  
structures (structs) and defined types (typedefs)

in C if you want to create a variable you have to do 2 things; specify data type and give name
you can declare more then 1 variable of the same data type with "," but you should only declare variables when you need them
  double doub, double, dloat; 

  int number; //declaration number as int
  number = 11; // assignment of number
  char character; // declaration character as char
  character = 'T'; // assignment of character, single quotes for single chaaracter (double quotes for multi characters, string type)
  int number = 11; // initialization - declaration and assignment in same line (instead of 2 lines like above
  float decimal = 11.7; // initialization
  
you only habe to declare your variable 1 time, weird things happen if you declare same variable multiple times

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Operators

Arithmetic Operators
add +
subtract -
multiply *
divide /
modulus %; //give remainder number

x = x * 5;
x *= 5;

increase x by 1
  x = x + 1
  x += 1
  x++ //x-- to decrease by 1
  
Boolean expressions
  comparing values
  evaluate one of two values - true or false
  used in conditionals and loops
    conditionals - deciding which path to take in a fork
    loop - deciding whether or not to continue the loop
  sometime in Boolean expressions we use variables with type bool, but it's not required
  in C every nonzero value is equivalent to true, and zero is false.
  
  two main types of Boolean expressions
    logical operators
      && - both variables have to be true
      || - OR, if either variable to true
      ! - NOT, x (true), !x (false)
    relational operators 
      < - less than
      <= - less than or equal to
      > - greater than
      >= - greater than or equal to
      == - equality, checks if the 2 variables have the same value
      != - inequality, checks if the 2 variables have different value
        = is assignment 
        == is equality
        DO NOT CONFUSE = AND ==

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------


  


  


























































































