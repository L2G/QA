# Mac OS GUI Validation

*DRAFT*

Submit completed tests and debug.log files to:  {Name &lt;email&gt;}

Version tested:
{0.x.y release candidate N, or git commit}

Test environment:
{Operating System or other relevant info}

## Test Setup

Describe any test environment setup that needs to be done, in an explicit, step-by-step fashion.

For example, for sanity-testing a release the setup might be:

0. Fork the test plan's github repository (see [TestPlanExecution.md](TestPlanExecution.md) )
1. Begin with a clean, non-developer operating-system image.
2. Download latest release candidate from sourceforge.
3. Run installer or follow installation instructions.
4. Create a bitcoin.conf file in the default data directory (~/.bitcoin on Linux, etc; see sample.bitcoin.conf)

## Tests

### Window close

1. Start Bitcoin-Qt.
2. Hit the window-close button.

EXPECT:

1. The window should close *and* Bitcoin-Qt should quit.
2. The dock should not show Bitcoin-Qt to be running (either no icon, or icon present without the "LED").

Choose one: PASS / FAIL

Comments: (add here if necessary)

### Final steps

Tell testers what they should do when they're finished; for example:

Email a link to your forked repository with attached debug.log files to {...}. If the debug.log files are
too large to attach, upload them to a service like mediafire.com, dropbox, etc. and include a link in the email.
