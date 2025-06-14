# 🛡️ Suricata IDS Lab – Real-Time Threat Detection

This is my Suricata IDS setup on Ubuntu, built to detect real-time network threats in a home lab environment.

---

## ✅ What I Did

- Installed Suricata on Ubuntu and ran it in **IDS mode** with `af-packet`
- Updated `HOME_NET` to `192.168.74.0/24` to match my local subnet
- Loaded and validated **43,000+ rules** with `suricata -T`
- Triggered a live alert using test traffic from `testmynids.org`
- Verified alerts in both `fast.log` and `eve.json`

---

## 🖼️ Screenshots

### 🧾 HOME_NET Config
![Image](https://github.com/user-attachments/assets/798670ae-d423-4bde-9ae1-e7e328b3b48f)


### ✅ Rule Validation
![Image](https://github.com/user-attachments/assets/dbf1c298-c9c7-487f-bcd6-1c787d7b68e8)

### 📡 Suricata Running in IDS Mode
![Image](https://github.com/user-attachments/assets/f5a48e4b-f329-473f-9ab8-5e91c755421d)

### 🚨 Detected Alert in fast.log
![Image](https://github.com/user-attachments/assets/68bdcc6c-5d2e-4f58-b460-971ca6794452)


---

##🧪 Test Traffic
I ran this command to simulate threat activity:

curl http://testmynids.org/uid/index.html

Resulted in this alert:

GPL ATTACK_RESPONSE id check returned root

🔜 Next Step
I'm now working on forwarding Suricata alerts to Wazuh for full SIEM integration.

👤 Author
Malik Bradley
🔗 LinkedIn: www.linkedin.com/in/malik-bradley-a1273b28a

