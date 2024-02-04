# Custom BCheck Scan

This repository stores some of my custom BCheck Scan configurations.
Its goal is to identify intriguing elements that warrant further manual testing.

Further information on [BCheck](https://github.com/PortSwigger/BChecks) can be found at the provided link.

## Repository Structure

The structure of this repository is as follows:

```bash
custom-bcheck-scan/
├── passives                   # Passive analysis on the response to identify elements worthy of further investigation.
├── common                     # Common check for misconfigurations for specific technology/framework/language
├── sensitive                  # Common check for sensitive file s
├── vulnerability-classes      # Specifically targeting a particular type of vulnerability such as sqli, xss, etc.
├── testing                    # Testing scan that I'm still experimenting with

```

## Testing the Scan

You have two options for testing the scan:

### Option 1: Import and Start Scanning
You can import all scans and begin scanning immediately.

### Option 2: Inspect Each Scan Using BSCode Editor
Follow the steps below to inspect each scan using the BSCode Editor:

1. Open BurpSuite and navigate to Extensions -> BCheck.
2. Click on 'New' -> Blank.
   ![BSCode Editor Window](bscode_editor_window_image.png)
3. Copy any scan into the editor.
4. Right-click on any request/response and select 'Send to BCheck Editor'.
   ![BSCode Editor Window](bscode_editor_window_image.png)
5. Click on 'Validate' to ensure the scan is correct, then click 'Run Test' to observe how the rule runs.

