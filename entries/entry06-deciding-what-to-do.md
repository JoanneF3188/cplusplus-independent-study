# Entry 6: Deciding what to do

This week, I was deciding on what I should do for my final project and I have
decided to work on small projects first. To start off, I decided that I would
create something that I have learned in class, a game of rock, paper, or scissors.

## What I Did

``` C 
#include <iostream>
#include <ctime> // Needed for the true randomization
#include <string>
using namespace std;

int comp()
{
    int rand_num;
    string comp_choice;
    srand( time(NULL)); // randomizes the number based off of time
    rand_num =rand()%3+1; // randomizes a number from 1 to 3
    
    if (rand_num == 1)
        comp_choice = "Rock\n";
    if (rand_num == 2)
        comp_choice = "Paper\n";
    if (rand_num == 3)
        comp_choice = "Scissor\n";
    
    cout << comp_choice;
    
    // return 0;
}

int user()
{
    string user_choice;
    cout << "Choose Rock, Paper or Scissor: ";
    getline (cin, user_choice);
    cout << user_choice << endl;
}

int main()
{
    user();
    comp();
}

// http://www.cplusplus.com/forum/beginner/98214/
// http://www.cplusplus.com/doc/tutorial/functions/
```

Currently, my code can only output the choice and the randomized choice. For my next steps,
I will attempt to find a way in which I can determine who is the winner or whether there is
a tie.

## Next Steps/Reminders

1. **Finished getting choices**
2. **Now, find a way to determine who wins and who loses OR ties**

## Takeaways
#### MVP
**!! It was a good idea to start off with smaller projects because once I have utilized the
code in my own way, I am able to be comfortable with using code that I can alter and tinker
with !!**

#### Google = BEST FRIEND
**I can't seem to emphasize enough that google is really a useful resource because throughout
this mini project, Google has helped me so much in finding the right code that I am unfamiliar with**

[**Back**](entry05-outputting-user-info.md) [**Menu**](../README.md) [**Next**](entry07-md) 