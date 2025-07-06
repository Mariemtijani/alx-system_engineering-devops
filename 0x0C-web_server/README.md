# 0x0C. Web server

## Project Description

This project focuses on automating the transfer of files from a local machine to a remote server using a Bash script. It demonstrates how to use `scp` with SSH keys and proper argument validation to securely copy files to a server's home directory.

### Task: 0. Transfer a file to your server

You are required to write a Bash script called `0-transfer_file` that:

- Accepts exactly 4 arguments:
  1. Path to the file to transfer
  2. IP address of the server
  3. Username to connect with
  4. Path to the SSH private key file
- Transfers the file to the remote user's home directory using `scp`
- Disables strict host key checking
- Displays a usage message if fewer than 4 arguments are passed

### Example usage

```bash
./0-transfer_file some_page.html 8.8.8.8 ubuntu ~/.ssh/id_rsa

