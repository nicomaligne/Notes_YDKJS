### Callbacks

single threaded (one at a time) event loop queue 

#### Continuation

async func are not blocking (captain obvious)
code following async call is executed
callback are executed at the end of the async call

#### Sequential brain

parallelism between the event loop vs the humain brain = very fast context switching

#### Doing versus planning

Brain are not deisgned to work in a async way so it makes difficult to understand naturally async code

#### Nest / chained callbacks

callback hell -> flow difficult to follow, complexed code and again hard time for the brain

#### Trust issues

using third party like ajax() is an inversion of control, we let the api take control of our code

#### Tale of Five Callbacks

callback hell meet third party api

#### Not Just Other's Code

We can control a simple way third api, callback hell need a lot of boilerplate / overhead code on every single callback to control the possible bug

#### Trying to Save Callbacks

different to try to save callback pattern
 - two function error and success ajax("url", success, failure) -> failure is optional, error can disapear...
 - node style = handle error first -> boilerplate and not enough control (with possible custom impl of timeout)
 - Don't release Zalgo -> sync-async hell -> make everything related async don't mix

 #### Review

 Callbacks is dead, ES6 bring more efficient async pattern