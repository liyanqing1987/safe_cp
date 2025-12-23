**Author:** liyanqing1987@163.com    
**Version:** V1.0 (2025.12.23)    
    
# What is “safe_cp”?
 
 `safe_cp` is a secure data copy tool, which works exactly the same as `cp`. It can be referenced in an alias manner or directly replace the system's cp command.

# Requirements

- Linux
- Python 3

# Quick Start

1.  use as alias    

     `[user@host ~]# alias cp=“/***/safe_cp“`    

2.  replace system cp

     `[root@host ~]# which cp`    
     `/usr/bin/cp`    
     `[root@host ~]# mv /usr/bin/cp /usr/bin/system_cp`    
     `[root@host ~]# cp safe_cp /usr/bin/cp`    

# Configuration

1. Recommended configuration    

     Specify protected path: `self.protected_path_list = ''`    
     Specify log directory: `self.log_dir = ''`    
     How to send alarm: `self.alarm_command = ''`    

2. Optional configuration    

     Specify protect path for yourself: `~/.config/safe_cp.protected`    


# Docs

More usage information please see [User Manual](safe_cp_user_manual.pdf)
