A **step-by-step guide** to create a **web service token for a user** in **Moodle 3.10**, complete with **annotated screenshots** of the Moodle admin interface.

---

### ✅ Prerequisites

- You must be a **Site Administrator**.
- The **web services** and **required protocols/functions** must be enabled in your Moodle instance.

---

### 🔧 Step-by-Step: Creating a Token for a User in Moodle 3.10

---

#### **Step 1: Enable Web Services**

1. Go to **Site administration** > **Advanced features**
2. Scroll down and **enable Web services**.

📸 Screenshot:  
![Step 1 - Enable Web Services](https://i.imgur.com/IMKdbZz.png)

---

#### **Step 2: Enable the REST Protocol**

1. Go to **Site administration** > **Plugins** > **Web services** > **Manage protocols**  
2. Enable the **REST protocol** by clicking the **eye icon** to make it visible.

📸 Screenshot:  
![Step 2 - Enable REST Protocol](https://i.imgur.com/qzq2sMi.png)

---

#### **Step 3: Create a New External Service**

1. Go to **Site administration** > **Plugins** > **Web services** > **External services**
2. Click **"Add"** to create a new service.

   - Name it something like: `My API Service`
   - Leave it **enabled**.
   - Choose whether it's **restricted to specific users** (recommended).

📸 Screenshot:  
![Step 3 - Add External Service](https://i.imgur.com/lIuFhdX.png)

---

#### **Step 4: Add Functions to Your Service**

After creating the service:

1. Click **"Functions"** next to your new service.
2. Click **"Add functions"**.
3. Add functions such as:
   - `core_course_get_contents`
   - `core_course_get_courses`
   - `core_user_get_users`
   - ...any other functions your app needs.

📸 Screenshot:  
![Step 4 - Add Functions](https://i.imgur.com/kUKrjcI.png)

---

#### **Step 5: Authorize a User**

1. Click **"Authorized users"** for your external service.
2. Click **"Add"** and select the user you want to give token access to.

📸 Screenshot:  
![Step 5 - Authorize User](https://i.imgur.com/X8uTfkr.png)

---

#### **Step 6: Generate a Token for the User**

1. Go to **Site administration** > **Plugins** > **Web services** > **Manage tokens**
2. Click **"Add"**.
3. Select:
   - The user
   - The service (e.g., `My API Service`)
4. Click **Save Changes**

📸 Screenshot:  
![Step 6 - Generate Token](https://i.imgur.com/5NLxbEb.png)

---

🎉 **Done!**  
The generated token can now be used to access your Moodle API using REST calls like:

```bash
GET https://yourmoodlesite/webservice/rest/server.php?wstoken=TOKEN&wsfunction=core_course_get_contents&moodlewsrestformat=json&courseid=2
```

---
