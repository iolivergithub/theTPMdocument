=== 22 April 2020 - Ian Oliver

The "perfect" trusted boot sequence, from power-on to running the code you want

x86 is complex
ARM is variable
Arduino ... an interesting idea - simple enough to understand.  What would make a Trusted Arduino ? 

=== 27 April 2020 - Dim Tomov

Make articles(examples) of how to build trust into the different components of a system

Based on our discussio at TPM.dev, everyone welcomed the System Architecture approach. Now the question is to define the big picture architecture and start adding content per category. Here is some idea about categories:
- Bootloader - What can we do to establish RoT (for measurement and reporting)
- Low-level runtime - What can we do to protect the loading of our OS/Kernel
- Normal runtime - What can we do to protect our user space OR How to make our normal execution environment more trusted
- Application level - Examples taht everyone can use to apply different TPM capabilities in their applicaitons

Based on suggestions from Paul and Daniel I started writing two articles/tutorials:
- How to use a TPM as True Random Number Generator and why it makes a difference?
- How to protect your private keys using a TPM?

I guess both of these fall into the Application category, although the second can be extended to TLS as recommended by Daniel.

=== 27 April 2020 - Ian Oliver

The trusted device lifecycle.... manufacturing->provisioning (OEMs, manufacturer, customer)->poweron->boot->load time->run-time->reboot->deprovisoning

Failures
