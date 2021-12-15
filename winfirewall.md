### Add inbound firewall rule for specific IP
New-NetFirewallRule -Name allow-inbound-192.168.0.125 -DisplayName 'allow-inbound-192.168.0.125' -Enabled True -Direction Inbound -Protocol ANY -Action Allow -Profile ANY -RemoteAddress 192.168.0.125

### Find Firewall rule by name
Get-NetFirewallRule -Name 'allow-*'