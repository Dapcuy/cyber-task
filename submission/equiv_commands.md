| No | Aksi                 | Linux (Ubuntu/Debian)                                   | Windows (PowerShell)                                                                                              |

| -- | -------------------- | ------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |

| 1  | Install package      | `sudo apt update \&\& sudo apt install -y <package\_name>` | `Install-Package -Name <package\_name>` (dengan PackageManagement / Chocolatey: `choco install <package\_name> -y`) |

| 2  | Start SSH service    | `sudo systemctl start ssh`                              | `Start-Service sshd`                                                                                              |

| 3  | Check service status | `systemctl status ssh`                                  | `Get-Service sshd`                                                                                                |

| 4  | Add firewall rule    | `sudo ufw allow 22/tcp`                                 | `New-NetFirewallRule -DisplayName "Allow SSH" -Direction Inbound -Protocol TCP -LocalPort 22 -Action Allow`       |

| 5  | View system info     | `uname -a \&\& lsb\_release -a`                            | `Get-ComputerInfo`                                                                                                |

