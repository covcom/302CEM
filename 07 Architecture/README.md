
# Architecture

Each week you will be expected to complete a series of lab activities. You will be required to reflect on these in your assignment so make sure you keep records of what you have done. The supporting presentation can be found at https://goo.gl/wwTHZK

## Sprint 3
You should be applying concepts covered in earlier labs to this sprint.

1. Your team have agreed a version control strategy and are refining this.
2. All completed user stories are backed by comprehensive acceptance tests that demonstrate success.

This sprint you have been learning about Unit Testing.

1. The app architecture of your current solution needs to implement MVC.
  1. Each platform uses different libraries to achieve this but typically for a dynamic website you should be using a templating solution, make sure your team have agreed which one they will use.
  2. As you modify your code this could break your product. Run the automated acceptance tests frequently to make sure nothing is broken!
2. You need to write comprehensive unit tests to cover the functionality in your current codebase. These tests will form your regression tests.
3. Now you can fully implement Test-Driven Development (TDD).
  1. In the technical planning agree on the public functions/methods in your code modules and their signatures.
  2. Write a comprehensive suite of unit tests that can be used to confirm functionality, these tests will fail when run.
  3. Implement the functionality in your modules and measure progress in terms of the number of tests that pass.

## Bugs
As you roll out your product to end users they will normally find bugs that need fixing. Use the process described below to report, track and fix them.

1. Ask other teams to represent your users. As they find bugs these must be added to the issue tracker. You will need to grant reporter access to the reporter access to the repository which will allow them to add bugs to the system.
2. Each bug needs to be rated for severity using the labels in GitLab and assigned to a developer for fixing.
3. If the team are implementing TDD, a bug represents a missing test.
  1. Create a branch in which the bug will be fixed, use the issue tracking number in the branch name.
  2. Write a Unit and/or acceptance tests to replicate the bug.
  3. Modify the code until all tests pass.
  4. Issue a merge request and assign to a different developer who will check the bug is fixed them merge the branch
  5. The issue is now closed in the issue tracker. This will notify the person who reported the initial bug.

## Microarchitecture
The lecture discussed how APIs can be used to build fully distributed systems. Take time to analyse your solution and identify where this approach could be used to improve the development of the product.

## Data Persistence
Reflect on your data-persistence options. How does the CAP theory impact on your choices?

## Messaging
How could message queues and pub-sub help decouple your system components?
