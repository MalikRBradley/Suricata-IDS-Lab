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
![suricata_t](./screenshots/suricata_t_validation.png)

### 📡 Suricata Running in IDS Mode
![suricata_running](./screenshots/suricata_running.png)

### 🚨 Detected Alert in fast.log
![Image](https://github.com/user-attachments/assets/68bdcc6c-5d2e-4f58-b460-971ca6794452)


---

## 🧪 Test Traffic

I ran this command to simulate threat activity:
```bash
curl http://testmynids.org/uid/index.html

