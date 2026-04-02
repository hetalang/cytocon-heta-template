# cytocon-heta-template

_This is draft package for Cytocon + 5db + Heta integration._

Public path to the certificate:

https://raw.githubusercontent.com/hetalang/cytocon-heta-template/main/certificates/heta-project-ss-cert.cer

## Contact
For questions or issues, contact **fivedb@insysbio.com**

## Installing the Certificate on Windows

To run the Excel XLSM file without security warnings, you must install the signing certificate once.

### Steps

1. Download the certificate file (`.cer`) using the link provided.

2. Double-click the downloaded certificate file.

3. Click **“Install Certificate…”**.

4. Select **Current User** *(Local Machine can be used if you have administrator rights)* and click **Next**.

5. Choose **“Place all certificates in the following store”** and click **Browse…**.

6. Select **Trusted Publishers**, then click **OK**.

7. Click **Next**, then **Finish**.

8. Confirm that the message **“The import was successful”** is displayed.

### Issues

If the certificate installation to **Trusted Publishers** does not resolve the issue, install the certificate to **Trusted Root Certification Authorities** at step (6) instead.

## Check Macro Settings in Trusted Center

After installing the certificate, verify the macro settings in **Trusted Center**.

### How to Open Trusted Center in Office 365 Excel

1. Open **Excel**.

2. Click **File** → **Options**.

3. In the left panel, select **Trust Center**.

4. Click **Trust Center Settings…**.

5. Open **Macro Settings** and review the current configuration.

### Recommended Check

Make sure that macro settings do not block signed macros from running.  
If needed, change the settings, then close Excel and reopen the XLSM file.

## Result

After installation, the XLSM file will open without certificate or macro security warnings.

> This installation is required only once per user or machine.

