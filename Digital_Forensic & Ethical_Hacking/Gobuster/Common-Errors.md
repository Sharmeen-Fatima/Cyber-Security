# Gobuster Common Errors and Solutions

## 📌 Introduction

While using Gobuster, you may encounter various errors related to installation, configuration, network connectivity, or command syntax. This guide explains the most common issues and how to resolve them.

---

# 1. Command Not Found

### Error

```bash
gobuster: command not found
```

### Cause

* Gobuster is not installed.
* Gobuster is not included in the system PATH.

### Solution

* Verify that Gobuster is installed.
* Restart your terminal after installation.
* Ensure the executable is available in your system PATH.

---

# 2. No Such File or Directory

### Error

```bash
Error: open wordlist.txt: no such file or directory
```

### Cause

The specified wordlist file cannot be found.

### Solution

* Check the file name.
* Verify the file location.
* Use the correct file path.

Example:

```bash
/home/user/wordlists/common.txt
```

---

# 3. Permission Denied

### Error

```bash
Permission denied
```

### Cause

The current user does not have permission to execute the command or access the required file.

### Solution

* Verify file permissions.
* Ensure you have appropriate access rights.
* If necessary, execute the command with the required privileges.

---

# 4. Connection Refused

### Error

```text
Connection refused
```

### Cause

The target server is not accepting connections.

### Solution

* Verify the target URL.
* Confirm that the service is running.
* Check network connectivity.

---

# 5. TLS / SSL Certificate Error

### Error

```text
x509: certificate signed by unknown authority
```

### Cause

The server is using an untrusted or self-signed SSL certificate.

### Solution

For authorized testing environments, you may use the appropriate Gobuster option to skip certificate verification when necessary.

---

# 6. Too Many Requests

### Error

```text
429 Too Many Requests
```

### Cause

The server is limiting the number of requests.

### Solution

* Reduce the number of threads.
* Add a delay between requests if appropriate.
* Wait before running another scan.

---

# 7. Timeout Error

### Error

```text
Request timeout
```

### Cause

The server did not respond within the configured timeout period.

### Solution

* Verify your internet connection.
* Increase the timeout value if appropriate.
* Confirm that the target service is reachable.

---

# 8. Empty Scan Results

### Problem

Gobuster completes the scan but does not find any resources.

### Possible Causes

* Incorrect target URL.
* Inappropriate wordlist.
* Requested resources do not exist.
* Server restrictions.

### Solution

* Verify the target.
* Try a different wordlist.
* Review the selected scan mode.

---

# 9. Invalid Command Syntax

### Error

```text
unknown command
```

### Cause

The command contains incorrect syntax or unsupported options.

### Solution

Review the Gobuster help page:

```bash
gobuster --help
```

---

# 10. DNS Lookup Failed

### Error

```text
no such host
```

### Cause

The domain cannot be resolved.

### Solution

* Verify the domain name.
* Check DNS configuration.
* Confirm that the domain exists.

---

# General Troubleshooting Tips

* Verify the installation before starting.
* Double-check command syntax.
* Ensure the correct wordlist is selected.
* Confirm that the target is reachable.
* Save scan results for later analysis.
* Read error messages carefully—they often indicate the root cause.

---

# Summary

Most Gobuster issues are related to installation, incorrect paths, network connectivity, or command syntax. Understanding these common errors will help you troubleshoot problems more efficiently and continue your authorized security assessments with confidence.
