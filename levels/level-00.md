# Bandit Level 0 — SSH Connection

## Objective

Establish a secure remote connection to the OverTheWire Bandit server using SSH (Secure Shell).

## Environment

- **Platform:** OverTheWire Bandit
- **Local operating system:** macOS
- **Remote operating system:** Linux
- **Protocol:** SSH
- **Port:** 2220

## Command Used

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

## Technical Explanation

- `ssh`: Initiates a secure remote connection.
- `bandit0`: Specifies the remote username.
- `bandit.labs.overthewire.org`: Identifies the remote server.
- `-p 2220`: Specifies a custom SSH port instead of the default port 22.

## Challenges Encountered

During the exercise, I attempted to establish another SSH connection while already logged into the remote server.

The server rejected the connection because SSH connections from localhost were restricted.

This helped me understand the difference between executing commands locally and remotely.

## Skills Acquired

- Establishing SSH connections
- Understanding SSH ports
- Identifying local and remote shell environments
- Interpreting terminal error messages
- Basic Linux command-line navigation

## Security Considerations

SSH provides encrypted remote access. Server host keys help verify the identity of the remote system.

Before trusting an unfamiliar SSH server, its host key fingerprint should be verified through a trusted source.

## Key Takeaway

Successfully connected to a remote Linux server using SSH and gained a better understanding of remote authentication and command-line environments.
