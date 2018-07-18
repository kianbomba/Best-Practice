# Unit Testing

There might be a rule of thumb of some people that each unit test must 
only have one -> two assertions per unit test. However, most of the times, I would prefer one assertion per unit test, 
because the name (**unit test**) itself is saying that it is a unit. 
Therefore, you should do one thing at a test. If it is too hard to not doing one assertion per test,
for example: `you are testing something in a loop`. You should consider about driving your test to fail at
some point within the loop that you are not expecting something. If your test is going through the loops
without failing and all the way down to the end of the test, at this point, you know that your test is passing,
and you do not have to do lots of assertion, but just one simple assertion at the end of the test

Each unit test should only test one function at a time, if you are testing multiple functions in one
test, then you should consider about you are **DOING UNIT TEST WRONG**. Unit test should be simple and fast, if
it requires a database connection layer or any kind of communications layer, then you should consider of
marking these tests as heavy test, so that it can be ran by the pipelines (or any sort of things in your workplace) 
and your co-worker can just run most of simple and light weight unit tests before they push any code to a master 
repository.

Unit test is an awesome tool that it could help you to detect a bug at an early stage. 
However, **DO NOT ABUSE UNIT TEST**, Unit tests can only assure 80% that your system is working.
If you want to have a perfect score, then you should consider integration test and manual test as well.
**DO NOT** obssess with the code coverage from your unit tests, it does not mean that 100% code coverage can
assure that your system is working flawless. You should keep this in mind that `the purpose of unit test is to prove
that each part of the system that you have made is going to the right direction base on the different
set of data you are injecting to it`.


I would rather spend time on writing tests than rushing things and have to spend more time on fixing the issues.
Learn unit test, and learn how to make it effectively.



Here are some extra sources that you might have interested in:

[Stackoverflow Query](https://stackoverflow.com/questions/3258733/new-to-unit-testing-how-to-write-great-tests)