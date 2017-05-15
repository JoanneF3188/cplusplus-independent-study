# Entry 7: Busy, Busy, Busy

<img src="../images/home-alone.gif"/>

Attack of APs!! Oh my goodness! This week has been quite busy so far. 
I am currently still stuck on attempting to find a way to who wins, 
loses OR ties. In my last weeks, I might end up creating a tutorial 
for my project mainly because the tutorials that I have found are pretty
old and it was hard for me as a beginner to understand. There has also
been code in which applies to old versions of C++ and then it gets all
sorts of confusing.

<img src="../images/confuzzled.gif"/>

## What I Did

```c
#include <iostream>
#include <ctime> // Needed for the true randomization
#include <string>
using namespace std;

int comp()
{
    int rand_num;
    string comp_choice;
    srand( time(NULL));
    rand_num =rand()%3+1;
    
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

//new code

int main()
{
    int user_choice;
    int comp_choice;
    user_choice = user();
    comp_choice = comp();
    
    if (comp_choice == "Scissor" && user_choice == "Paper" || comp_choice == "Rock" && user_choice == "Scissor" || comp_choice == "Paper" && user_choice == "Rock")
    cout << "Computer wins!!";
}
```

## Brain Thoughts
`cin.get();` = wait for user to press enter key
<!--http://www.cplusplus.com/forum/general/39982/-->


## Takeaways
#### Take your time to read EVERYTHING
As we get more and more busy with trying to finish our projects, we will be 
tempted to want to just skip and rush over eveything. Sometimes, we just need
to take some time and slowly read everything to make sure we understand each
line of code.

[**Back**](entry06-deciding-what-to-do.md) [**Menu**](../README.md) 
<!--[**Next**](entry08-.md) -->