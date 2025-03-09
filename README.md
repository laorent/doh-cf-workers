# 🚀 Cloudflare Encrypted DNS Worker Setup Guide 🚀

## ⚠ Disclaimer ⚠

🔹 **This project is an open-source initiative designed to build a DNS over HTTPS (DoH) forwarding service using Cloudflare's Worker functionality.**

🔹 **The goal is to enhance network privacy and security, providing users with a more secure and privacy-protected DNS resolution service.**

📌 However, users must acknowledge the following disclaimers:

1️⃣ **This project is strictly for technical research and personal use.** It must not be used for any activities that violate laws, regulations, or infringe on others' rights.

2️⃣ **This project utilizes Cloudflare's Worker functionality as infrastructure but is NOT officially maintained or endorsed by Cloudflare.** Cloudflare bears no responsibility for any damages caused by its use.

3️⃣ **The authors and contributors disclaim liability for any issues arising from this project,** including but not limited to:
   - Data loss
   - Service interruptions
   - Network security vulnerabilities

4️⃣ **Users must comply with all applicable internet-related laws and regulations** and take full responsibility for their actions.

5️⃣ **If any individual or organization misuses this project to harm Cloudflare’s interests or violate its terms of service,** the authors and contributors bear no responsibility. All legal liabilities rest solely on the perpetrators.

📢 **Users should carefully read and understand this disclaimer before using the project. By proceeding, you agree to abide by all its provisions.**

---

# 📖 User Guide: Creating an Encrypted DNS Worker on Cloudflare

## 1️⃣ Create a Worker on Cloudflare

✅ **Log in** to your Cloudflare account and go to the Dashboard.  
✅ **Select** `Workers` from the navigation bar at the top.  
✅ **Click** on `Create a Worker` to start setting up your Worker.

---

## 2️⃣ Copy the DoH Worker Code

✅ **Open** the project on GitHub and locate the `doh-cf-worker.js` file.  
✅ **Copy** all the code from the file (`Ctrl+C` or `Command+C`).  
✅ **Return** to the Cloudflare Worker editor and **paste** the code (`Ctrl+V` or `Command+V`).  
✅ **Click** `Save and Deploy` to finalize deployment.

📌 **If you find this project helpful, please consider giving it a ⭐ on GitHub to support further development!**

---

## 3️⃣ Bind a Custom Domain

✅ **In the Cloudflare Worker editor**, navigate to the `Route` tab.  
✅ **Click** `Add Route` in the Route section.  
✅ **Enter** your custom domain (e.g., `example.com`).  
✅ **Specify** the `/dns-query` path so that requests will be directed to `example.com/dns-query`.  
✅ **Click** `Save` to apply the settings.

---

## 🌐 Using Encrypted DNS

✅ **Open** your browser settings and navigate to the DNS settings.  
✅ **Enter** your custom domain with the `/dns-query` path (e.g., `example.com/dns-query`).  
✅ **Save** the settings, and your browser will start using the encrypted DNS service provided by your Cloudflare Worker.

---

📢 **For further assistance or troubleshooting, refer to the Cloudflare documentation or contact their support team.** 🚀

📌 **Remember to ⭐ Star the project on GitHub if you find it useful!**

