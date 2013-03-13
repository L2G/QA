# Mac OS GUI Validation

*DRAFT*

This document is designed to be copied and pasted into a GitHub issue ticket, from the "Environment"
heading on down.

## Test Setup

Describe any test environment setup that needs to be done, in an explicit, step-by-step fashion.

For example, for sanity-testing a release the setup might be:

0. Fork the test plan's github repository (see [TestPlanExecution.md](TestPlanExecution.md) )
1. Begin with a clean, non-developer operating-system image.
2. Download latest release candidate from sourceforge.
3. Run installer or follow installation instructions.
4. Create a bitcoin.conf file in the default data directory (~/.bitcoin on Linux, etc; see sample.bitcoin.conf)

## Environment

Version tested:
{0.x.y release candidate N, or git commit}

Test environment:
{Operating System or other relevant info}

## Tests

*Note:* Open pairs of brackets are included for convenience: when pasted into an issue or pull request, these turn the
lists into checklists.

### Main window: close

***Steps:***

1. [ ] Start Bitcoin-Qt.
2. [ ] Click the window-close button.

***Expect:***

1. [ ] The application quits completely.

***Result:*** (choose one)

* [ ] PASS
* [ ] FAIL

***Comments:*** (add here if necessary)

### Preferences: Window tab

***Steps:***

1. [ ] Start Bitcoin-Qt.
2. [ ] Open Preferences and choose "Window."

***Expect:***

1. [ ] All checkboxes are shown as disabled.
2. [ ] No checkbox can be ticked.

***Result:*** (choose one)

* [ ] PASS
* [ ] FAIL

***Comments:*** (add here if necessary)

### Final steps

Tell testers what they should do when they're finished; for example:

Email a link to your forked repository with attached debug.log files to {...}. If the debug.log files are
too large to attach, upload them to a service like mediafire.com, dropbox, etc. and include a link in the email.
