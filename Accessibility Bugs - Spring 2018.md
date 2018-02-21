**CS 490 - Homework**
This document was used in the fall 2017 version of CS 490 Software Engineering at Western New England University. The table may be updated as bugs are fixed or closed. 

**Bug Tracking - 20 Points**

The Mozilla Dev Tools communityhas provided us with a list of possible bugs to work on:

https://github.com//issues?q=is%3Aissue+is%3Aopen+label%3Aaccessibility

You must explore the list of bugs and fill out the table below according
to:

  - **Dependent On** - List the number of any bugs upon which the
    current bug is dependent.

  - **Related To** - List the number of any related bugs mentioned in
    the bug report.

  - **Community** - List the names of any communities that must be
    consulted when solving the bug.

  - **Hints for Solving** - Identify any hints, directions or solutions
    provided in the bug report.

  - **Status -** Select one of the status terms:
    
      - **Wait** - The solution cannot be completed until some action is
        taken by someone in the community
    
      - **Go** - The solution can be created with no further input
        needed from the community

      - **Claimed** - Issue has been claimed and is in progress.
    
      - **Question** - There are unresolved questions within the bug
        report that require answers from the
        
      - **Closed** - The issue was either closed or the solution is no longer needed.
community


|  Bug No.  | Status      | Depends On  |  Related To  | Community | Hints for Solving |
| --------- | ----------- | ----------- | ------------ | --------- | ----------------- |
| #4181     | Go          |             |              |           |                   |
| #4078     | Claimed (Berea) |         |              | Designer  | Is implementing the "focus ring" a short term solution? Sample code provided.  |
| #4076     | Question    |             |              | Chrome DevTools, Edge teams | |
| #4075     | Claimed (Berea) |         |              |           | Explanation of solution provided by Garbee. Sample code provided.  |
| #4080     | Claimed (Berea) |         |              |           | Sample code provided. Some question as to what terms mean.  |
| #4070     | Claimed (Berea) |         | #4071        |           | Example code provided  |
| #4071     | Requested closed |        | #4070        |           | Example code provided  |
| #4067     | Requested closed | #695 - blocker | #4081, #4068 |   | Solution might be in m-c. Jason indicated he would update #695 soon.  |
| #4073     | Closed      |             |              |           | Explanation of solution provided by Garbee. Sample code provided.  |
| #4068     | Closed      |             | #4081        |           | Same solution as for #4067. Requires updating to latest devtools-core tree component. See comment on #4067 |
| #4081     | Closed      |             | #4067, #4068 |           | One comment suggested closing the bug.  |

[jlast](https://devtools-html.slack.com/team/U3UH6CSLR#_blank)

[7:39
PM](https://devtools-html.slack.com/archives/C3VTFTCBY/p1505777957000083#_blank)

oh great. yeah, the student should provide lots of
feedback

[7:39](https://devtools-html.slack.com/archives/C3VTFTCBY/p1505777959000106#_blank)

[https://github.com//issues/4080](https://github.com//issues/4080#_blank)

![](media/image1.png) GitHub

[accordion accessibility · Issue \#4080 ·
](https://github.com//issues/4080#_blank)

This issue tracks the work to make the accordion accessible. A PR can do
one or several items in the checklist: Visually (CSS focus styling)
there is no way to focus on the accordion headers and
...

![](media/image2.png)

[7:39](https://devtools-html.slack.com/archives/C3VTFTCBY/p1505777988000176#_blank)

^ I left some notes in a comment, but would love to get your thoughts /
input as
well

[7:40](https://devtools-html.slack.com/archives/C3VTFTCBY/p1505778010000195#_blank)

[@victoria](https://devtools-html.slack.com/team/U5E02H0AH#_blank) what
do you think would be a good focus state for accordion headers?
