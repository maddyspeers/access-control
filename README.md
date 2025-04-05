# Rogue Access Point Attack - Mitigation Plan  
**Group 12:** Brianna Deaubler, Madelyn Speers, Angelin Benny, Daut Hadzijusufovic  
**Course:** CIS4219 - Human Aspects of Cybersecurity  
**Date:** November 18, 2024  

## 📌 Overview  
This README outlines our team’s mitigation strategy for defending against a rogue access point (AP) attack in a mid-sized organization located in a secure, multi-floor building. While physical security is strong, the lack of a Network Access Control (NAC) system created a gap that led to the theft of corporate trade secrets. After thorough analysis, we evaluated three solutions and selected **MAC address filtering** as the most practical, cost-effective option to enhance network security.

---

## 🧠 What is a Rogue AP?  
A **rogue access point** is an unauthorized device connected to a network, potentially allowing attackers to bypass security and access sensitive information. These can be installed physically or remotely and are often used to steal data by mimicking trusted network devices.

---

## 🔍 Incident Summary  
- **Cause:** A rogue AP was likely connected to an unused Ethernet port or configured using a company device.  
- **Vulnerability:** Lack of NAC system despite high physical security.  
- **Impact:** Theft of trade secrets and exposure of internal network.

---

## 🛡️ Mitigation Techniques Considered

### 1. Intrusion Prevention System (IPS)  
- **What it does:** Real-time monitoring and blocking of malicious traffic.  
- **Tools:** Open-source solutions like Snort.  
- **Pros:** Automated detection, real-time alerts, works well in Ethernet environments.  
- **Cons:** Moderate cost, ongoing maintenance, potential false positives.

### 2. MAC Address Filtering ✅ *(Chosen Solution)*  
- **What it does:** Allows only pre-approved MAC addresses to connect to the network.  
- **Pros:** Moderate cost, strong control over device access, effective in a physically secured environment.  
- **Cons:** Requires ongoing list management, vulnerable to MAC spoofing.

### 3. Employee Cybersecurity Training  
- **What it does:** Educates employees on detecting rogue APs, phishing, and social engineering.  
- **Pros:** Low cost, raises awareness, improves overall cyber hygiene.  
- **Cons:** Not foolproof, dependent on employee engagement and retention.

---

## ✅ Why We Chose MAC Address Filtering  
MAC address filtering offered the best **balance between security and cost**. With a well-managed list of company-owned devices and strong physical access controls already in place, this method gives us direct control over network access without major budget or infrastructure changes.

---

## 🛠️ Implementation Highlights  
1. **Register Devices:** Collect and verify MAC addresses of all approved company devices.  
2. **Configure Access Points/Switches:** Restrict connections to registered MACs.  
3. **Policy Enforcement:** Regularly update address lists as devices are added or removed.  
4. **Monitoring:** Set up alerts for unauthorized access attempts.  
5. **Routine Audits:** Perform checks to detect spoofing attempts and ensure list accuracy.

---

## 💡 Supplementary Measures  
Although MAC filtering was chosen as the main solution, **IPS** and **employee training** will be considered as secondary reinforcements to create a multi-layered defense strategy. Together, these techniques help defend against both technical and human-based threats.

---

## 📚 References  
[1] "What is a rogue access point & how to protect against them," Nilesecure. [Online]. Available: https://nilesecure.com/network-security/what-is-a-rogue-access-point-how-to-protect-against-them  
[2] "What is an intrusion prevention system (IPS)," Palo Alto Networks Cyberpedia. [Online]. Available: https://www.paloaltonetworks.com/cyberpedia/what-is-an-intrusion-prevention-system-ips  
[3] "Intrusion prevention system (IPS)," VMware. [Online]. Available: https://www.vmware.com/topics/intrusion-prevention-system  
[4] "Snort," Fortinet Cyberglossary. [Online]. Available: https://www.fortinet.com/resources/cyberglossary/snort  
[5] "Intrusion prevention system (IPS)," GeeksforGeeks. [Online]. Available: https://www.geeksforgeeks.org/intrusion-prevention-system-ips/  
[6] "Integrated product support (IPS) elements overview," DAU Acquipedia. [Online]. Available: https://www.dau.edu/acquipedia-article/integrated-product-support-ips-elements-overview  
[7] R. S. Ross, M. McEvilley, and J. C. Oren, “Systems security engineering: Considerations for a multidisciplinary approach in the engineering of trustworthy secure systems,” NIST SP 800-160, vol. 1, NIST, 2016. Available: https://doi.org/10.6028/NIST.SP.800-160v1  
[8] S. R. Tate and K. S. Trivedi, "MAC address filtering: Practical implications and limitations," in Proc. IEEE Conf. Comput. Commun. Workshops (INFOCOM WKSHPS), Apr. 2018. doi: 10.1109/INFCOMW.2018.8407012  
[9] T. A. Fulford, "Security considerations and challenges in MAC-based filtering techniques for modern networks," IEEE Trans. Netw. Serv. Manag., vol. 16, no. 3, pp. 764–774, Sept. 2019. doi: 10.1109/TNSM.2019.2921918  
[10] L. Xie, K. Kang, and J. H. Park, "Security and privacy in IEEE 802.11 wireless local area networks: A comprehensive survey," IEEE Commun. Surveys Tuts., vol. 19, no. 4, pp. 2876–2924, 2017. doi: 10.1109/COMST.2017.2732991  
[11] A. Salah, H. D. Chen, and Y. Lin, “Assessment of MAC address filtering effectiveness in small enterprise networks,” in Proc. 15th Int. Conf. Netw. Security (ICNS), Oct. 2017. doi: 10.1109/ICNS.2017.8046812  
[12] F. Wang and Z. Li, "Evaluation of physical and logical access control in secure environments: Lessons for modern organizations," IEEE Access, vol. 8, pp. 204032–204041, 2020. doi: 10.1109/ACCESS.2020.3038064  
[13] "AI-powered, new-school security awareness training," KnowBe4, 2024. [Online]. Available: https://www.knowbe4.com  
[14] CISA, "Cybersecurity training and exercises," 2024. [Online]. Available: https://www.cisa.gov/cybersecurity-training-exercises  
[15] HHS, "Security awareness training," 2024. [Online]. Available: https://www.hhs.gov/about/agencies/asa/ocio/cybersecurity/security-awareness-training/index.html  
[16] Center for Internet Security (CIS), "Why employee cybersecurity awareness training is important," 2024. [Online]. Available: https://www.cisecurity.org/insights/blog/why-employee-cybersecurity-awareness-training-is-important  
[17] Verizon, "2024 Data Breach Investigations Report," 2024. [Online]. Available: https://www.verizon.com/business/resources/Taf9/reports/2024-dbir-data-breach-investigations-report.pdf  

