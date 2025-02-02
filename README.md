# GCP IAM, Storage, and Compute Engine Hands-On Lab

## 🚀 Overview
In this project, I document my hands-on experience with **Google Cloud IAM**, **Cloud Storage**, and **Compute Engine** access control, focusing on setting up users, roles, and permissions to maintain secure access.

---

## 🔹 Step 1: Creating IAM Users
To start, I created two IAM users for testing roles and permissions in the Google Cloud Console:

- **User-1**: `student-00-2e30b4fa0498@qwiklabs.net`
- **User-2**: `student-00-591f96ac3a3b@qwiklabs.net`

![Creating IAM Users](https://github.com/user-attachments/assets/33398e28-a676-43f6-8f8f-b88560a8b9a8)

---

## 🔹 Step 2: Assigning IAM Roles
I assigned the following IAM roles to **User-2** to ensure proper permissions:
- **Viewer** (read-only access to project resources)
- **Storage Object Viewer** (read-only access to Cloud Storage)

![Assigning IAM Roles](https://github.com/user-attachments/assets/e6edab31-daa1-49fa-b3f2-44a99f16fbc9)  
![Role Assignment Confirmation](https://github.com/user-attachments/assets/a1ea9361-a47e-42d6-8fa1-af6dd5be001a)

---

## 🔹 Step 3: Creating a Cloud Storage Bucket
Next, I created a **Cloud Storage Bucket** to experiment with object access control.

![Cloud Storage Bucket Creation](https://github.com/user-attachments/assets/feae899c-cf19-4287-89d9-183109cc2197)

---

## 🔹 Step 4: Uploading and Managing Objects
I uploaded a test file and renamed it within the storage bucket for practice.

![Uploading File](https://github.com/user-attachments/assets/4da09541-5cfa-4f43-956d-090d7e64e319)  
![Managing Object](https://github.com/user-attachments/assets/704a2fc3-5b87-40d4-84e9-ea1533872790)  
![Renaming Object](https://github.com/user-attachments/assets/c3b86f4a-6266-457b-8d1e-f93626958ff6)  
![Object Renamed](https://github.com/user-attachments/assets/8a4e9101-46d4-425f-b280-96475590efe5)

---

## 🔹 Step 5: Verifying Access with Cloud Shell
To verify access, I used the `gcloud storage ls` command to ensure **User-2** could list files in the storage bucket.

![Verifying Access in Cloud Shell](https://github.com/user-attachments/assets/7edb1ddc-c40f-4460-835a-6244d6acdf9f)

---

## 🔹 Step 6: Creating a Service Account
I created a service account (`read-bucket-objects`) with the **Storage Object Viewer** role to manage permissions securely.

![Creating Service Account](https://github.com/user-attachments/assets/eca385f3-e703-444f-ac16-2f2a396578d8)  
![Service Account Permissions](https://github.com/user-attachments/assets/e41a290b-5d15-4902-baca-88c563f13413)  
![Service Account Confirmation](https://github.com/user-attachments/assets/8cb8e95a-2527-4ba8-b30c-efa5cd59a558)

---

## 🔹 Step 7: Assigning the Service Account to Compute Engine
To ensure secure access to compute resources, I assigned the service account to a **Compute Engine VM**.

![Assigning Service Account to Compute Engine](https://github.com/user-attachments/assets/75b41f2a-c810-4c5b-a236-fa7c6bbe7d9a)  
![Service Account with Compute Engine](https://github.com/user-attachments/assets/fb8f7e80-e1f1-42e9-bbba-93be99524866)

---

## ✅ Conclusion
This hands-on lab provided valuable experience in configuring **IAM roles**, **Cloud Storage permissions**, and **Compute Engine access control**. Key takeaways:
- Configured **user roles** and **service accounts** following the **principle of least privilege**.
- Verified user access and permissions with the **gcloud CLI**.
- Gained knowledge on **restricting VM access** using a controlled service account.
- Enhanced understanding of **Google Cloud security best practices**.

I am now confident in managing access control for Google Cloud resources and implementing security best practices.

---


