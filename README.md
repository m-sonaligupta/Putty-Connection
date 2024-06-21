# Putty-Connection
## Connecting to an Instance Using PuTTY

This guide will help you connect to your server instance using PuTTY, a free and open-source terminal emulator.

---

### Step 1: Download and Install PuTTY

**Download PuTTY:**
- Visit the official [PuTTY Download Page](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html).
- Download the appropriate version for your operating system.

**Install PuTTY:**
- Run the downloaded installer.
- Follow the on-screen instructions to complete the installation.

---

### Step 2: Obtain Your Instance's IP Address and SSH Key

**Instance IP Address:**
- Find your instance's IP address from your cloud provider's management console (usually labeled as Public IP or Public DNS).

**SSH Key:**
- Download your instance's SSH private key file (`.pem` file) from your cloud provider.

---

### Step 3: Convert the .pem File to a .ppk File Using PuTTYgen

**Open PuTTYgen:**
- Launch PuTTYgen from the Start menu.

**Load Your .pem File:**
- Click on **Load**.
- Select **All Files (\*.\*)** from the file type dropdown.
- Locate and select your `.pem` file.

**Save the Key:**
- Click on **Save private key**.
- You can choose to save without a passphrase, though it's more secure to use one.
- Save the file with a `.ppk` extension.

---

### Step 4: Configure PuTTY to Connect to Your Instance

**Launch PuTTY:**
- Open PuTTY from the Start menu.

**Enter Host Name:**
- In the **Host Name (or IP address)** field, enter your instance's IP address.

**Specify the .ppk File:**
- In the **Category** pane, expand **SSH** and select **Auth**.
- Click **Browse** and select your `.ppk` file.

**Save the Session:**
- Go back to the **Session** category.
- Enter a name for the session in the **Saved Sessions** field and click **Save**.

---

### Step 5: Connect to Your Instance

**Select Your Saved Session:**
- In the PuTTY Configuration window, select your saved session and click **Load**.

**Initiate Connection:**
- Click **Open**.
- If prompted, accept the security alert.

**Login:**
- A terminal window will open.
- Login using the username provided by your cloud provider (e.g., `ubuntu` for Ubuntu instances, `ec2-user` for Amazon Linux).

---

Congratulations! You are now connected to your instance using PuTTY.

For further details and troubleshooting, refer to the [PuTTY Documentation](https://www.chiark.greenend.org.uk/~sgtatham/putty/docs.html).

