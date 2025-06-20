# 🚀 Mandatory-Tag-Policy-Implementation-for-EC2-using-AWS-Organizations

This project demonstrates how to **enforce mandatory tags** during the launch of EC2 instances using **AWS Organizations**, **Tag Policies**, and **Service Control Policies (SCPs)**. It ensures governance, accountability, and cost management across AWS accounts by blocking EC2 instance creation without the required metadata tags.

---

## 📌 Project Objectives

- ✅ Create and enable an AWS Organization
- ✅ Create and apply EC2 mandatory **tag policies**
- ✅ Attach policies to organizational accounts
- ✅ Launch EC2 instances **with and without tags** to observe enforcement behavior
- ✅ Confirm enforcement of **lowercase keys** (case sensitivity)
- ✅ Ensure only **tag-compliant EC2 instances** are allowed

---

## 🔧 Required EC2 Tags (Enforced)

| Key       | Example Value                  |
|-----------|--------------------------------|
| `name`    | Yuvrani                        |
| `emailid` | yuvranirandive1@gmail.com      |
| `phoneno` | 9355165480                     |
| `place`   | Pune                           |

> ⚠️ **Note**: All keys must be lowercase due to case sensitivity in the tag policy.

---

## 📁 Project Structure

### 🔨 Tasks Completed

- ✅ **Organization Created**
- ✅ **Tag Policy Created**
- ✅ **Tag Policy Attached** to Management Account
- ✅ **Service Control Policies Enabled**
- ✅ **EC2 Mandatory Tag Enforcement Enabled**
- ✅ **EC2 Instance Launched with Tags** — ✅ Success
- ❌ **EC2 Launch Without or Incorrect Tags** — Blocked with error
- ✅ Final EC2 Instance is running successfully 🎉

---

## 📄 Sample JSON: EC2 Tag Policy

```json
{
  "tags": {
    "name": {
      "enforced_for": ["ec2:instance"]
    },
    "emailid": {
      "enforced_for": ["ec2:instance"]
    },
    "phoneno": {
      "enforced_for": ["ec2:instance"]
    },
    "place": {
      "enforced_for": ["ec2:instance"]
    }
  }
}


## 📸 Screenshots

Below are the key screenshots captured during the implementation of this project:

| 📷 Step | Description |
|--------|-------------|
| ✅ **1.** | Creation of AWS Organization |
| ✅ **2.** | Enabling Service Control Policies |
| ✅ **3.** | Creation of EC2 Mandatory Tag Policy |
| ✅ **4.** | Attaching Tag Policy to the AWS Account |
| ✅ **5.** | Additional Tags Attached While EC2 Launch |
| ✅ **6.** | EC2 Instance Launch Attempt with Incorrect Tag (`Name` instead of `name`) |
| ✅ **7.** | EC2 Instance Launch Error (Tag Policy Enforcement Worked) |
| ✅ **8.** | Successful EC2 Launch with All Required Tags |
| ✅ **9.** | Running EC2 Instance Screenshot |
| ✅ **10.** | Final Completion of the Project with Tag Policy in Effect |

📝 _You can find these screenshots inside the `screenshots/` folder of this repository._

---

## 🧠 Learnings

- Learned how to enforce organizational tagging policies using **AWS Tag Policies**
- Understood the **case sensitivity** involved in tag key enforcement
- Explored how **Service Control Policies (SCPs)** can restrict EC2 instance launches
- Identified challenges in SCP attachment and used a fallback approach with tag policies
- Gained hands-on experience in **governance, compliance, and cost control** strategies using AWS native tools

---

## 🛡 Tech Stack

- **Amazon EC2** – Launching and testing virtual instances
- **AWS Organizations** – Setting up policies across accounts
- **Tag Policies** – Enforcing tagging compliance for EC2 instances
- **Service Control Policies (SCPs)** – Optional attempt to block unauthorized EC2 launches
- **IAM Policies (Optional)** – Evaluated for permission-based controls
- **AWS Management Console** – End-to-end configuration
- **Markdown / GitHub** – For reporting and documentation

---

## 🏁 Final Output

- ✅ Successfully launched EC2 instances with **all mandatory tags**
- ❌ Attempted EC2 launches without required tags were **blocked or errored** as expected
- 🛡 Organizational tag enforcement was demonstrated using **Tag Policies**
- 🎯 Project demonstrates a **real-world use case** of cloud resource governance using native AWS features

---

## 📌 Author

**👩‍💻 Yuvrani Randive**

- 🎓 Electronics & Telecommunication Engineering Graduate  
- 🌐 [LinkedIn Profile](https://www.linkedin.com/in/yuvranirandive)  
- 📧 yuvranirandive1@gmail.com  
- 💡 Passionate about Cloud Computing, DevOps, and Cloud Governance

---



