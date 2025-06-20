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

## 📸 Screenshots
Below are the key screenshots captured during the implementation of this project:

📷 Step	Description
✅ 1.	Creation of AWS Organization
✅ 2.	Enabling Service Control Policies
✅ 3.	Creation of EC2 Mandatory Tag Policy
✅ 4.	Attaching Tag Policy to the AWS Account
✅ 5.	Additional Tags Attached While EC2 Launch
✅ 6.	EC2 Instance Launch Attempt with Incorrect Tag (Name instead of name)
✅ 7.	EC2 Instance Launch Error (Tag Policy Enforcement Worked)
✅ 8.	Successful EC2 Launch with All Required Tags
✅ 9.	Running EC2 Instance Screenshot
✅ 10.	Final Completion of the Project with Tag Policy in Effect

📝 You can find these screenshots inside the screenshots/ folder of this repository.

📁 Folder Structure
📦 aws-ec2-tag-enforcement
┣ 📂 screenshots
┃ ┣ 1-org-created.png
┃ ┣ 2-scp-enabled.png
┃ ┣ 3-tag-policy-created.png
┃ ┣ 4-policy-attached.png
┃ ┣ 5-ec2-tag-added.png
┃ ┣ 6-name-tag-error.png
┃ ┣ 7-tag-error-message.png
┃ ┣ 8-launch-success.png
┃ ┣ 9-instance-running.png
┃ ┗ 10-project-completed.png
┣ 📄 README.md
┣ 📄 ec2-tag-policy.json
┗ 📄 report.md or report.pdf

🧠 Learnings
Enforced tagging standards using AWS Tag Policies

Understood the importance of case-sensitive key enforcement

Explored Service Control Policies (SCPs) and their limitations

Used tag policies for resource governance and compliance

Managed EC2 instances with automated tag validation

🛡 Tech Stack
Amazon EC2

AWS Organizations

Tag Policies

Service Control Policies (SCP)

IAM

AWS Management Console

GitHub + Markdown for documentation

🏁 Final Output
✅ EC2 instance successfully launched with required tags

❌ Launches without tags were blocked, verifying policy enforcement

🎯 Demonstrated effective AWS cloud governance via tag policy compliance

📌 Author
👩‍💻 Yuvrani Randive
🎓 Electronics & Telecommunication Engineering Graduate
🌐 LinkedIn
📧 yuvranirandive1@gmail.com
💡 Passionate about Cloud Computing, DevOps, and AWS Governance



---



