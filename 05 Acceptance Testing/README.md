
# Acceptance Testing

Each week you will be expected to complete a series of lab activities. You will be required to reflect on these in your assignment so make sure you keep records of what you have done. The supporting presentation can be found at https://goo.gl/JxMDl5

## Regression Testing
In your first sprint, you devised a set of detailed, manual tests to verify that your code solved the user story. You will now learn the concepts and syntax of the testing framework for your chosen platform by writing a set of tests to prove your code has passed.

1. Write detailed acceptance tests that describe the user story you have finished
  1. Write tests that test correct input
  2. Write tests that test incorrect input
2. Make sure all the tests pass

## Sprint Review
The current sprint is ending so you will need to perform a review.

1. Form a standing group around a (large) monitor.
  1. Make sure all the team are present.
  2. Make sure one of the academic lab staff is also present.
2. The Product Owner reads out the user story.
3. One of the team demonstrates that this has been fully implemented by showing the working software (don't use the automated tests).
4. The product owner and customers present try out the new features and ask questions which need to be clearly answered by the team.
5. If the product owner and customers are happy with the working product, it is signed off.
6. If there are concerns there are two options:
  1. If the solution fails to deliver any benefits the user story is replaced at the top of the product backlog.
  2. If the solution partially works, the team, together with the customer write a new user story to fill in the gaps.
7. Issues are discussed and a solution established to prevent these issues recurring.
8. The planning meeting now needs to be carried out for the next sprint.

## Sprint Planning
You are now ready to run your second sprint planning meeting. Assign the roles of Scrum Master and Product Owner to different team members.

1. Carry out the same process as described in the previous labs.
2. If you are collaborating with other teams you should run a combined planning meeting.
3. Go through the product backlog and use MoSCoW rules to re-order the cards based on input from the team.
4. Take the top-most card and use BDD rules to design a suitable technical solution.
  1. Design the interface (use a whiteboard or paper)
  2. Iteratively design the architecture using the BDD process.
5. Divide up the work between members of the team.
  1. Members should be assigned work in their skill area.
  2. Ideally each task should be assigned to a pair of developers.

## Test-Driven Development
Instead of writing out a sequence of manual tests to ensure compliance your team will practice TDD.

1. Create a feature branch for the user story.
2. Extend the existing acceptance tests you wrote earlier to write detailed tests.
3. Run the tests, they should fail.
4. Start your feature development.
5. Re-run your test suite regularly to check what still needs to be implemented.

## Supporting Materials

There are a number of supporting labs that will help you implement your acceptance tests.

1. If you are creating a **website**, use the materials in the **casperjs** directory.
2. If you are creating an **API**, use the materials in the **frisbyjs** directory.