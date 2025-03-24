# Understanding OWASP: Preventing Security Misconfigurations and Real-World Threats

Group Members:
Nur Shakirah I'zzah Zamri
Nursyahmina Mosdy
Syamilia Nur Najwa Mohd.syahiram
Umairah Natasha Zainal Abidin
Nurfarisha Kamarrudin

Lecturer:
Cik Feresa Mohd Foozy

# 1.	Introduction of OWASP

The Open Worldwide Application Security Project (OWASP) is a nonprofit foundation focused on enhancing software security. It provides knowledge, tools, and community-led projects to assist organizations in developing, maintaining, and operating secure software applications. OWASP's objective is critical in today's digital landscape, where cyber threats are constantly developing, requiring comprehensive application security. One of OWASP's most well-known initiatives is the OWASP Top 10 which is a standard awareness document that highlights the ten most serious security dangers to web applications. This list is a core resource for developers and organizations, assisting them in recognizing and addressing common vulnerabilities. The OWASP Top 10 is updated every few years to include new security risks and trends. The changes are based on data from security studies and real-world attacks. As of 2024, the next update (OWASP Top 10:2025) is planned for the first half of 2025, with an emphasis on emerging threats. The updated 2025 LLM Top 10 highlights dangers like unbounded consumption, vector or embedding vulnerabilities, and system prompt leakage, and also provides guidelines on safeguarding these modern technologies.

# 2.	Risks and Prevention of Security Misconfiguration

Believe it or not, the most common cyber threat is as simple as security misconfiguration. This happens when security isn't configured strongly enough, unneeded features stay enabled, or default settings aren't changed. It's similar to leaving a spare key under the welcome mat and knowing the hackers do too. Think of default credentials, for example. Most web applications use default passwords and usernames like "admin" for both the password and username fields. Another common error is directory listings or having very detailed error messages shown. While they might not appear to be an issue, these can inadvertently leak sensitive information, making a hacker's job much easier. Worse still, insecure admin panels, improper security headers, or loose settings in APIs and web frameworks can offer an opening for unauthorized access. Attackers prey on these vulnerabilities, looking for open admin panels, default password testing, or exploiting poor configurations. One incorrect setting is all that is required for hackers to gain access, so rechecking security settings is imperative.

There are various ways attackers can exploit security misconfigurations, typically by scanning for vulnerabilities or testing weak points manually in application. One of the common methods is through automated tools that checks for outdated software. Attackers often use the tools to check the software version before looking for known exploits of that version. They might also execute techniques like code injection by injecting malicious code or scripts into the application due to a company's failure to update its software on time and patch its security flaws. Lastly, exploitation could also happen through unencrypted files. It usually results in a major risk to users. Attackers who gain access to the system or information can easily read and alter the data. All files that contain sensitive information should always be encrypted to add a layer of protection. Without the correct decryption key, the data remains secure and indecipherable even when breached illegally. 

Fixing security misconfigurations can start with pretty straightforward but necessary steps. To illustrate, the developers need to take the time to turn off unnecessary features and set default options because small things make a difference. Another significant step is locking down authentication, like using multi-factor authentication to protect sensitive sections. It is similar to having a second lock on your main door, easy but a worthwhile layer of protection.
For error messages, a pinch of customization is magic. Instead of showing complete system information, which could help attackers, developers need to ensure error messages show only what's necessary. Proper configuration of security headers such as Content Security Policy (CSP) and HTTP Strict Transport Security (HSTS) also helps prevent potential exploits. Developers can also use security configuration management (SCM) tools, automated security testing and regular updates to protect their web applications from security misconfigurations. To help detect misconfigurations and implement security policies, SCM tools are great to be used by developers. System hardening reduces attack surfaces by applying strict access controls and disabling unnecessary services. Automated tools like OWASP ZAP scan for vulnerabilities, while regular updates prevent exploitation of outdated software.
 
# 3.	A Real-World Web Security Breach

In 2017, the incident that considered one of the largest data breaches in the country’s history. Malaysia has experienced a data breach that exposed the personal details of around 46.2 million mobile subscribers. What happened in the breach was, the breach involved the unauthorized exposure of sensitive information, that includes mobile numbers which both active and inactive numbers were leaked. Not only that, but there were also leaks of personal details such as home address's identity card numbers (MyKad), and SIM card information. Other than that, there were also leaks of International Mobile Equipment Identity (IMEI) and International Mobile Subscriber Identity (IMSI) numbers.
Major Malaysian telecom companies, including Maxis, DiGi, Celcom, and others, had their subscribers included in the hacked data. Interestingly, there were more compromised records than Malaysia's 32 million people, indicating that the incident involved several numbers per person, inactive numbers, and temporary numbers that tourists had bought.

# How does the breach relate to the selected OWASP risk?

These can lead to security misconfiguration occurring when the system or the applications are poorly secured, which leaves them vulnerable to exploitation. For the case of the Malaysian data breach, the problem most likely resulted from system configuration errors at the impacted telecom providers that gave unauthorized users access to private information. Even though the exact nature of the misconfiguration was not revealed, such as vulnerabilities commonly included to let the systems with insecure default settings, failing to apply the necessary security patches and giving people or systems unduly lenient access permissions. These types are consistent with the OWASP Top 10 security risks under the category of Security Misconfiguration.

# What Could Have Prevented the Attack?

To mitigate security breaches, organizations must adopt a proactive and layered approach to cybersecurity. The following measures can significantly reduce the risk of attacks:
    
# 1.	Regular Security Audits
-	To find flaws in networks, apps, and systems, do thorough penetration tests and vulnerability assessments.
-	To find configuration errors, exposed services, and out-of-date software, combine manual reviews with automated scanning tools (such as Nessus, Qualys, and OpenVAS).
-	Analyse logs to keep an eye out for odd activity that might point to a breach.
-	Arrange for independent assessments of security posture through third-party audits.

# 2.	Timely Patching
-	To guarantee that all operating systems, firmware, and software are updated on time, implement a patch management policy.
-	Apply critical patches (like those for zero-day vulnerabilities) as soon as possible and adhere to a specified SLA (such as 24 to 72 hours for high-risk vulnerabilities).
-	To expedite updates throughout the company, use automated patch management tools (such as WSUS, SCCM, and Ansible).
-	To prevent interruptions, test patches in a staging environment prior to deployment.

# 3.	Configuration Management
-	Adopt security baselines to make sure systems are protected from attacks (e.g., NIST guidelines, CIS Benchmarks).
-	To enforce consistent and secure configurations, use infrastructure-as-code (IaC) and configuration management tools (such as Ansible, Puppet, and Chef).
-	Maintain constant configuration monitoring to identify drift (unauthorised modifications) and automatically correct deviations.
-	To lessen the attack surface, turn off unused services and default credentials.
