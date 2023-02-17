# 10. Overview of any software validation conducted and by whom

1. A SW specification is written for the new feature
1. The feature is implemented based on the specification
1. A request is created to merge the feature to the main development branch
1. Iterative process is started to review and test the new feature
    1. Existing automated tests are run to verify that the new feature doesn’t break anything and is safe to merge
    1. Possible new automated tests implemented with the feature are run to verify that the feature works according to specification
    1. The new code is reviewed by other developers
    1. The new feature is tested by the reviewers and/or testers depending on the feature
    1. The new code is updated according to the review comments
1. The pull request is approved and merged to the main development branch
1. The new tests are merged as part of the automated tests
1. Final automated tests are run to verify that noting is broken in the main development branch