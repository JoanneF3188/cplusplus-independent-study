# Entry 4: The Exploring
This week, I went more in depth to the syntax of C++. In the previous entry, I had a few
questions that I was curious about. While learning the syntax, I wondered why programmers
preferred to use one line of code over the other. Therefore, I decided that I needed to do
some research before I can use C++ to it's full extent. I knew that I would feel a lot more
comfortable using the code when I know the reasons why a programmer would use a line of code.

## What I learned/Questions Answered
**Question:** Why use endl if \n is easier to write?
* `std::endl` flushes the output, meaning that it will immediately perform the line of code.
Typically, this is used when displaying output from a long-running process, logging activity
of multiple threads or logging activity of a program that may crash unexpectedly. 
[CPP Reference](http://en.cppreference.com/w/cpp/io/manip/endl)

* Programmers normally use `\n` over `std::endl` in situations that are unnecessary because
it worsens the performance of the output. So, programmers use `\n` more often than `std::endl` 

## Brain Thoughts/Questions to Answer


* Cool starting programs to code
1. [](http://projects.icbse.com/cpp-170)
2. [](https://www.quora.com/What-are-some-cool-small-C++-programs#)

## Takeaways


[**Back**](entry03-starting.md) [**Menu**](../README.md) [**Next**](entry05-.md) 

### References

* [CPP Reference](http://en.cppreference.com/w/cpp/io/manip/endl)
* [Stack Overflow](http://stackoverflow.com/questions/213907/c-stdendl-vs-n)
* 