# SCRCIssueTracking

Issue tracking for all models in the Scottish Covid Response Consortium.

The reason that this is a standalone repo for issues is that some projects are forks, which don't allow their own issues, and that some issues are cut across multiple projects and need some level of interoperability.

Please be aware that this means you must take care when referencing issues by number in commit messages - trying to may inadvertantly reference an issue in the original repository that the repo in this org was forked from. To correctly refer to  issue from within a commit message it have the full path, e.g. `ScottishCovidResponse/SCRCIssueTracking#123`, but only in the description (not the first line of the commit) i.e.

- `git commit -m "pithy description" -m "ScottishCovidResponse/SCRCIssueTracking#123 and more details"` to refer to issue number 123. 

- writing the commit messageand description in an editor is also possible with `export EDITOR=vi` for example, and then just doing a `git commit`. 
- bash also recognises line breaks in the double inverted commas

```bash
￼$ git commit -m "first line
￼>
￼> second line ScottishCovidResponse/SCRCIssueTracking#123"
```


**Please use labels:** We are establishing a labelling system that will let us filter issues down for various purposes and this will become more important as the number of issues increases. Please set up a label for each model and use that to mark all its specific issues. Other labels established so far (initially by James Cook and Claire Harris for the Julia project) are to help categorise tasks and identify those that are ready for new contributors to start on etc. The lead RSE for each project should adopt and add to these as needed and we can confer via Zulip if we need to refine the system.
