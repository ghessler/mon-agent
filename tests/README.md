Tests for the mon agent.

Run with `nosestests -w tests`

For many tests to work an agent.conf must be in either /etc/mon-agent/agent.conf or in the working directory.

Many tests require specific applications enabled in order for the test to run, these are skipped by default. See
https://nose.readthedocs.org/en/latest/plugins/skip.html for details.