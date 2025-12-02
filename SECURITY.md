# Security Policy

## How to Report Security Issues and Vulnerabilities

At HomeDock OS Desktop, your security is our **top priority** even while it's still a Beta. If you discover any vulnerabilities or security issues, please report them directly to our security team at:

📧 **support@homedock.cloud**

We deeply value the contributions of our community in making HomeDock OS Desktop a secure and reliable platform. Thank you for helping us improve!

---

## Security Update History

- `✦ Unauthenticated RCE via Docker Engine API CSRF (Windows)`

  - **Reported at Secur0 by m2rc** – Fixed in v0.44.682
  - Malicious websites could execute arbitrary code via CSRF attacks targeting the Docker API proxy on port 2375 on Windows. Now uses randomized ports with HTTP header validation to block browser-originated requests.

- `✦ Local Privilege Escalation via VHDX Path Hijacking (Windows)`

  - **Reported at Secur0 by m2rc** – Fixed in v0.43.196
  - Insecure handling of VHDX file paths could allow a local attacker to escalate privileges by manipulating the Docker virtual disk detection mechanism on Windows. Migrated and reimported previous VHDX files on the fly to secured paths.

- `✦ Remote Code Execution via Port Parameter Injection (Windows)`

  - **Reported at Secur0 by m2rc** – Fixed in v0.43.195
  - Malicious cloud instances could inject arbitrary commands through unvalidated port parameters in exposed IPC handlers. Now validates all port inputs and restricts sensitive operations to local origins only.
