Fun fact : I/O is async -> console.log is async :)

#### Event loop

JS engine run in a hosting environment (mobile, browser etc...)

One main thread -> event loop = one loop one tick / on demand execution

Scheduled event -> ajax call -> response -> callback

#### Parallel threading

JS do not share data across threads == deterministic (if code is ok)

#### Run to completion

code inside func == atomic
when func start -> finish before next operation

#### Concurrency

JS can handle one thing at a time
JS can have multiple task / process at the same time

#### Noninteracting

Two process using the same data but don't mutate it for example
It's non determistic but acceptable 

#### Interaction

Using condition / cheking data we can add deterministic behavoir

#### Cooperation

Slice chunk of code to allow in between func

#### Jobs

Job queue at the end of the event loop queue
Add a task at the end of the tick before the next tick

#### Statement ordering

At compile time JS reorganize code to run faster = safe optimization