# Parallo CES Offering

This project provides a streamlined way to deploy Azure resources using ARM templates. It includes an Azure "Deploy to Azure" button in the `index.html` file, which references the ARM template located in the `arm-templates` folder.

## Project Structure


### Key Components

1. **ARM Templates**:
   - The `arm-templates` folder contains the ARM templates required for deploying Azure resources.
   - The primary template is `sub-ces-foundation.json`, which defines the resources and configurations for the deployment.

2. **Azure Deploy Button**:
   - The `index.html` file includes a "Deploy to Azure" button.
   - When clicked, it redirects to the Azure portal and uses the ARM template specified in the `index.html` file for deployment.
   - The button references the `sub-ces-foundation.json` template hosted on GitHub.

### How to Use

1. **Serve the Project Locally**:
   - Run the following command to serve the project locally:
     ```bash
     python -m http.server 8000
     ```
   - Open `http://localhost:8000` in your browser to access the "Deploy to Azure" button.

2. **Deploy the ARM Template**:
   - Click the "Deploy to Azure" button in the browser.
   - This will open the Azure portal with the [sub-ces-foundation.json](http://_vscodecontentref_/3) ARM template preloaded for deployment.

### Notes

- Ensure the ARM template URL in the [index.html](http://_vscodecontentref_/4) file is correct and points to the hosted version of the [sub-ces-foundation.json](http://_vscodecontentref_/5) file.
- The ARM template includes parameters for configuring the deployment, such as `mspOfferName`, `mspOfferDescription`, and `managedByTenantId`.

