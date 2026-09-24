# Access ASPIRE 2B

Access to ASPIRE 2B is via an SSH (Secure Shell) client to login nodes.

## Login Nodes
| FQDN |
| :--- |
| aspire2b.nscc.sg |

## Access Instructions
1. Launch CheckPoint VPN client. If you do not have checkpoint VPN client, please refer to [Checkpoint Install Guide](https://help.nscc.sg/aspire2B/user-guide/)
2. Via CheckPoint VPN client, connect to vpn2.nscc.sg (DUO 2FA auth required)
3. Run the following command with your preferred terminal tool. Replace ```<userid>``` with your NSCC user ID.
  ```
  ssh <userid>@aspire2b.nscc.sg
  ```
