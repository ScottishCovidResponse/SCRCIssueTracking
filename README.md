# SCRCIssueTracking

Welcome to the issue tracking repository for the Scottish COVID-19 Response Consortium.

## Issue tracking

### Why a standalone repo?

The reason that there is a standalone repo for issues is that we anticipate that once the models are fully functional then some discussions may contain sensitive information. Having a standalone issue repository allows us to make it private to accommodate that, while simultaneously allowing us to ensure that the codebases and their associated repos can always remain public. Some issues also cut across multiple projects and need some level of interoperability, and this will help with that. However we appreciate there are downsides to this approach, and we discuss workarounds below - more suggestions are welcome.

### Referencing issues

Please be aware that having an issue repository separate from the code repo means you must take care when referencing issues by number in commit messages and PRs - trying to reference an issue using just `#123` may not resolve, or may inadvertently reference an issue in the original repository that the repo in this org was forked from. To correctly refer to an issue from within a PR or a commit message it must have the correct path to the issue on the `ScottishCovidResponse/SCRCIssueTracking` repository. An autolink reference should have been created in each repository to make a shortcut: `ScottishCovidResponse/SCRCIssueTracking#123` -> `SCRC-123`. Please put the reference in the commit description (not the first line of the commit) i.e.:

- `git commit -m "pithy description" -m "SCRC-123 and more details"` to refer to issue number 123.

- writing the commit message and description in an editor is also possible with `export EDITOR=vi` for example, and then just doing a `git commit`.

- bash also recognises line breaks in the double inverted commas

```bash
$ git commit -m "first line
>
> second line SCRC-123"
```

### Labels and Projects

We are establishing a [labelling system](https://github.com/ScottishCovidResponse/SCRCIssueTracking/labels) that will let us filter issues down for various purposes and this will become more important as the number of issues increases, as well as a series of [projects at the organisational level](https://github.com/orgs/ScottishCovidResponse/projects) to keep track of progress for each group. Please (set up and) use the label and project for each model to mark all its specific issues. Other labels established so far (initially by James Cook and Claire Harris for the Julia project) are to help categorise tasks and identify those that are ready for new contributors to start on, etc.

### Teams

We also have a series of [teams](https://github.com/orgs/ScottishCovidResponse/teams) to give control over the individual repos and projects. This is largely because there are a lot of people with access to this organisation who have no experience of git or github, and we want to make sure nothing bad happens by accident! 

## Discussions and problems

We have no doubt that we've made mistakes while setting all of this up! Apologies in advance - it was done in a rush. In particular, you may not be a member of the right teams, so you may not have write access to the right repos or projects, or autolinking may not be set up for a repo. You will have automatic access to our [Zulip](https://zulip.scrc.uk) workspace (a Slack-like service) through membership of the `ScottishCovidResponse` github organisation. Please use it to ask for help or if you find other glitches as we get all of this working smoothly. We also welcome suggestions for how to improve the ease of use for all of us!

In any event, the lead RSE for each project should adopt and add to what is already set up as needed and we can confer via Zulip if we need to refine the system - each project should have its own stream on Zulip shortly. If yours doesn't, please ask on `#general` for it to be set up.

### Problems

If you have any problems with the above that aren't easily resolved on Zulip, please raise issues tagged with the [Admin](https://github.com/orgs/ScottishCovidResponse/projects/2) project and the [Admin & management](https://github.com/ScottishCovidResponse/SCRCIssueTracking/labels) label.
