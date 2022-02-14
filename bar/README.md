`BAR_PRIVATE_KEY` -> The private key of `bar`.

`VPS_PUBLIC_KEY` -> The public key of the VPS.

`VPS_PUBLIC_IP` -> The public IP address of the VPS.

**If `bar` is a windows machine then comment out `PreUp` and  `PostDown` lines, those lines enable IP forwarding on linux machines, on windows you can enable `RemoteAccess` service and start it using this command on powershell (with administrative privileges):**

```
Set-Service -Name RemoteAccess -StartupType Manual -Status Running
```