# Task 1: Set Up Basic Firewall Rules

## Task: Configure firewall settings on a personal computer.
Enable and configure Windows Defender Firewall or a similar firewall.  
Set rules to block or allow specific applications or ports.

## Steps

### 1. Open Windows Defender Firewall
- Navigate to the **Control Panel**.
- Click on **System and Security**.
- Select **Windows Defender Firewall** to open the firewall settings.
!(./images/1.png)

### 2. Access Advanced Settings
- On the left-hand panel, click on **Advanced Settings**.
- This opens the **Windows Defender Firewall with Advanced Security** console, where detailed firewall configurations can be made.

### 3. Create Inbound Rules

#### a. Block Specific Ports
- In the left-hand panel, select **Inbound Rules**.
- Click on **New Rule...** in the right-hand Actions panel.
- Choose **Port** and click **Next**.
- Select **TCP** or **UDP**, and enter the port number (e.g., 21 for FTP).
- Click **Next**, select **Block the connection**, and click **Next** again.
- Choose when the rule should apply (**Domain**, **Private**, **Public**), then click **Next**.
- Name the rule (e.g., "Block FTP Port 21") and click **Finish** to apply the rule.

#### b. Allow Specific Applications
- In the left-hand panel, select **Inbound Rules**.
- Click on **New Rule** in the right-hand Actions panel.
- Choose **Program** and click **Next**.
- Browse to the application's executable file (e.g., `C:\Program Files\Browser\browser.exe`).
- Click **Next**, select **Allow the connection**, and click **Next** again.
- Choose when the rule should apply (**Domain**, **Private**, **Public**), then click **Next**.
- Name the rule (e.g., "Allow Web Browser") and click **Finish** to apply the rule.

### 4. Create Outbound Rules

#### a. Block Unnecessary Traffic
- In the left-hand panel, select **Outbound Rules**.
- Click on **New Rule...** in the right-hand Actions panel.
- Choose **Program** or **Port**, depending on the traffic to block, and click **Next**.
- Specify the program or port to block and click **Next**.
- Select **Block the connection**, and click **Next**.
- Choose when the rule should apply (**Domain**, **Private**, **Public**), then click **Next**.
- Name the rule (e.g., "Block Unnecessary Traffic") and click **Finish** to apply the rule.

### 5. Test the Configuration
- Test the configuration by attempting to access the blocked application or port to confirm that the rules are functioning as expected.
- Ensure that allowed applications are able to function properly.

## Outcome
The system was successfully configured with customized firewall rules that:
- Block specific ports and unnecessary traffic.
- Allow essential applications to function without interruption.
