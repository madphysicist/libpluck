libpluck
========

A library for plucking ripe CPU cores

Any competent computer user knows that CPUs become ripe with usage. This is usually an effect of moving dirty memory into the cache as non-sequential instructions are executed. Individual cores, and eventually the entire CPU become ripe with usage. If not plucked in time, cores can go bad, or spoil in technical parlance, with disastrous results for perfomance and reliability of the entire machine, not just the affected program.

Most users rely on random pieces of code called "pluckers" which align themselves in such a fortuitous manner that they effectively undo the effects of dirty memory. Unfortunately conincidental pluckers usually do not occur frequently enough to fully compensate for the accumulated RAM garbage, eventually requiring a periodic reboot of every machine.

The purpose of this library is to provide an indispensable service known as plucking. It contains routines for polling the available cores to determine when they ripen. It will pluck the affected cores before they have a chance to spoil. This distribution comes with a daemon program that runs the polling in the background... forever, since your cores will never spoil again!

A note to end-users:
This library requires enterprise-level hardware to run successfully. The more professional and advanced, the more successfully it will perform its function.
