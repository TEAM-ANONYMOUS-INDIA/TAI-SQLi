# Advanced SQL Injection Scanner

![TAI SQLi Banner](https://i.ibb.co/5BtLqk4/Screenshot-20250111-100048-Termux.jpg)

> ⚡ **Made by TEAM ANONYMOUS INDIA** ⚡  
> 🔥 **The Ultimate SQL Injection Scanner** 🔥  
> **Use this responsibly and ethically** ⚡

---

## Features
- **Multi-threaded Testing**: Test multiple payloads concurrently for faster results.
- **Blind SQL Injection**: Time-based detection for blind SQL injection vulnerabilities.
- **WAF Bypass**: Bypass techniques to evade Web Application Firewalls.
- **Automatic Parameter Detection**: Automatically detect SQL injection parameters in URLs.
- **Colorful Output**: Enhanced, readable output with color-coded messages.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/TEAM-ANONYMOUS-INDIA/TAI-SQLi.git
   cd TAI-SQLi

2. Install the required dependencies:

pip install requests colorama




---

Usage

Basic Command:

python3 sql_scanner.py -u <target_url> -p <parameter> [options]

Available Options:

-u <url>
Specify the target URL with a parameter to test for SQL injection.
Example: -u "http://example.com/page?id=1"

-p <parameter>
The parameter to inject for SQL testing.
Example: -p "id"

-m <method>
The HTTP request method to use. Default is GET.
Choose between GET or POST.
Example: -m POST

-t <threads>
The number of threads to use for faster testing. Default is 10.
Example: -t 20

-b
Enable blind SQL injection testing (time-based).
Example: -b

-f
Automatically detect SQL parameters in the URL.
Example: -f

-w
Enable WAF bypass techniques to avoid detection.
Example: -w



---

Example Commands

1. Basic SQL Injection Test (GET Method):

python3 sql_scanner.py -u "http://example.com/page?id=1" -p "id"

2. SQL Injection Test (POST Method):

python3 sql_scanner.py -u "http://example.com/login" -p "username" -m POST

3. Blind SQL Injection Test:

python3 sql_scanner.py -u "http://example.com/page?id=1" -p "id" -b

4. Automatically Detect SQL Parameters:

python3 sql_scanner.py -u "http://example.com/page?id=1&user=admin" -f

5. Enable WAF Bypass Techniques:

python3 sql_scanner.py -u "http://example.com/page?id=1" -p "id" -w


---

Example Output

When testing a vulnerable parameter:

[*] Target: http://example.com/page?id=1
[*] Method: GET
[*] Threads: 10

[+] Vulnerable! Payload: ' OR '1'='1 --

When no vulnerability is found:

[*] No SQL Injection vulnerability detected.


---

Legal Disclaimer

This tool is intended for educational purposes only. You are required to have explicit permission to test the websites. Unauthorized testing may be illegal and unethical.

Use this tool responsibly!


---

Contributing

We welcome contributions to improve this tool. Feel free to submit a pull request for bug fixes, improvements, or any other suggestions!


---

License

This project is licensed under the MIT License.

### Key Changes:
1. **Flag Descriptions and Examples**: These are now listed sequentially rather than in a table format. Each option is followed by a description and an example.
2. **Formatting**: Clean and easy-to-follow instructions, with an improved layout for a better reading experience.
3. **Banner**: Retained the image as requested.
4. **GitHub Link**: Correct GitHub repository link is included (`https://github.com/TEAM-ANONYMOUS-INDIA/TAI-SQLi`).

Let me know if you need further adjustments!

- **Formatting**: Cleaned up and made the layout more user-friendly, ensuring the README is easy to read and navigate.
- **GitHub Link**: The GitHub repository link is updated to `https://github.com/TEAM-ANONYMOUS-INDIA/TAI-SQLi`.
