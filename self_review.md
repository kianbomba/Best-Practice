# Self Review Checklists

#### Easy stuff
* Check all the files you did not mean to or need to change.

* Removing the debug statements and dead code.

* Fix coding styles issue (are you not following the code convention or not ?)

#### Regression and side-effects
* Look at each change in your Pull/Merge request, and ask yourself
whether this change could break somewhere else in the system or not ?
(if you could have asked this, you are already a PRO !!!)

#### Corretness
* Make sure that your code does what it needs to.

* Make sure you have your tests to prove or protect your changes.
It does not have to be just unit test, if it is hard to do unit test, write an integration test
instead. However, most of the times, unit test is more preferable, as it is fast and it makes more
sense than integration test (Selenium sucks !)

* Make sure all the tests (both unit and integration) of your system are passing. 
If not, your change is breaking somewhere else in the system

#### Quality
* Is your code easy to read or understand ? Ask yourself this more often,
as we are developers/programmers are really lazy. Therefore, we always end up doing everything
in one go (a * function with thousands lines of code), which will cause the complexity of the code and system.

* Did you choose the best name and organize your code ? Make sure you are writing
 an obvious code to your co-worker.
 
 * Is there any tricky logic that you have implemented ? If there is, make sure you put
 nice comments explaining about what is happening in that logic. Otherwise, after a 
 period of time you would even forget what you have implemented