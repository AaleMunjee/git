## Changing the `.yml` file

#### Introduce Changes to the `.yml` File

We've created more tests on the in the `/tests` directory. Let's go through the process of adding a new test, and seeing what it's like to break it or test it.

1. If you look in the `tests/` directory, you'll see a few new tests. We're going to add the `tests/test_speedmax.rb` test to the `.yml` file.
1. Create a new branch based on `gh-pages`.
1. On that branch, open the `.yml` file. Add `tests/test_speedmax.rb` to the file in the same place that the other test, checking the URL, is being run.
1. Create a pull request.
1. Review the contents of the new test. What do you think it does? Why would we implement it? What could we do differently? When will it pass or fail?

#### Break the Speed Test

1. Based on what you know about that test file, make a change that you think will cause the test to fail. (Change line 78 `min:` to be anything outside of `0.0` and `1.0`.)

#### Enable Protected Branches
1. See that you _could_ merge the pull request even though the tests are failing.
1. In your repsitory, click on the `Settings` tab.
1. Select `Branches` on the left navigation panel.
1. Under `Protected Branches`, click `Choose a branch` and select `gh-pages`.
1. Select `Protect this branch` and then select whichever protections you'd like for your default branch.


#### Fix the Speed Test
1. After the status check returns from the CI/CD service, fix the file so the tests pass.
1. Merge the pull request.
