# Mothlight honeypot data

Live SSH attack data from the [Mothlight](https://github.com/realzephaniahjohnson/mothlight) Cowrie honeypot
(Oracle Cloud, Montreal). Updated every 5 minutes. Shown live at https://mothlight.streamlit.app.

**Last update:** 2026-11-21 20:30 UTC · **235,428 events** from **1,570 attacker IPs** · 82,091 login attempts
(last 7 days, newest 300,000 events at most)

`honeypot.csv` columns: `timestamp`, `src_ip`, `event`, `username`, `password`, `command`, `session`

`event` is one of `login_failed`, `login_success`, `command`, or `download` (`command` holds the URL).
Every row is an attack against a fake SSH server. The usernames and passwords are ones that attackers
tried, not real credentials. Our own IPs, ports, and private traffic are removed before publishing.
