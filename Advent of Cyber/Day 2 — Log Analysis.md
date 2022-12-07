### Common Locations of Log Files

#### Windows

Windows has an in-built application to access historical records of events [Event Viewer]

Events are categorized as following:
- Application
- Security
- Setup
- System

#### Linux (Ubuntu/Debian)

Operating system log files are located within`/var/log` directory

- Authentication
- Package Management
- Syslog: events related to background tasks like crontabs.
- Kernel: events related to kernel events like changes to kerne; or output from networking equipment or physical devices (USB)

### Grep 101

By default, `grep` will use your current working directory.

Common flags:
- `-i`: case insensitive search
- `-E`: search using regex
- `-r`: recursive search 




