# April 10, 2024

Okay, so here's the deal. I wanted to setup Pi-Hole, and failed.

By default, Android 11+ has that "Private DNS" setting set to "Automatic", which means that instead of using normal DNS, it will use DNS over TLS (DoT). DoT works on port 853, and needs a valid domain name and TLS certificate, which thus means having dynamic DNS setup for certificate renewal. Also, pi-hole doesn't support DoT by default, so it needs a gateway like `dnsdist`, or switching to AdGuard. This is a lot of moving parts, lots of failure modes, high complexity and I thus believe it to be a high maintenance setup, which is what I'm trying to avoid if I want a reliable setup for my home internet access.

I failed to find a simple solution, but at least our Android phones can reach the web \o/
