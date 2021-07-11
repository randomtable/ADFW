# ADFW
GPO profiles for your systems

This Repository Contains GPOs you can apply for your managed systems.

# ADFW Profile
The ADFW Profile is very restrictive.

You can use this Profile for jump servers or critical systems.

You have to modify this policy to fit your organizational requirements, for example:
- Users can reboot or shutdown hosts
- Only the user "utente" can logon on the system
- Only "putty.exe" on the "utente" Desktop can run
- The DC "10.0.0.1" can communicate with the host freely, all TCP and UDP ports are opened
- Despite the rule above, WMI and management, RDP and other communications are not allowed (you have to run "gpupdate /force" on the host to update policies, for example)
- The Lab Domain is "dominio.it"

I suggest to create a lab and test/modify this policy before apply it on production systems.

I will update this project with a more complete wiki and some examples.

I will upload more profiles that covers different needs.

Let me know.
