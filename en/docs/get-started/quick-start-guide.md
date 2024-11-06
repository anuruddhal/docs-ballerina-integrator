## Overview
In this guide, you'll build a simple integration using the Kola plugin for Visual Studio Code. You'll create an HTTP service with a single resource named `greeting` that invokes the public [Hello World API endpoint](https://apis.wso2.com/zvdz/mi-qsg/v1.0) and returns the response.

<a href="{{base_path}}/assets/img/get-started/introduction.png"><img src="{{base_path}}/assets/img/get-started/introduction.png" alt="introduction" width="70%"></a>

### Step 1: Install Visual Studio Code
Download and install the [Visual Studio Code](https://code.visualstudio.com/download).

### Step 2: Create a profile in Visual Studio Code.
1. Open the Visual Studio Code.
2. Navigate to **Settings**->**Profile**->**Profiles**.
3. Click on **New Profile** dropdown and select **Create Profile**.
4. Enter the profile name as `Kola` and click **Create**.
5. Click on the ✔️ sign in front of the `Kola` profile to select the profile.   
   <a href="{{base_path}}/assets/img/get-started/create-profile.gif"><img src="{{base_path}}/assets/img/get-started/create-profile.gif" alt="Create Profile" width="70%"></a>

!!! info "Profile"
    To learn more about profiles, see [Visual Studio Code Profiles](https://code.visualstudio.com/docs/editor/profiles).

### Step 3: Install the Kola extension.
1. Go to the Extensions view by clicking on the extension icon on the sidebar or pressing `Ctrl + Shift + X` on Windows and Linux, or `shift + ⌘ + X` on a Mac.
2. Search for `Kola` in the Extensions view search box.
3. Click on the **`Install`** button to install the `Kola` extension.
   <a href="{{base_path}}/assets/img/get-started/kola-extension.png"><img src="{{base_path}}/assets/img/get-started/kola-extension.png" alt="Kola Extension" width="70%"></a>
4. This will install Kola, KolaB extension to the Visual Studio Code IDE.

### Step 4: Setup Kola for the first time.
1. Click on the Kola icon on the sidebar.    
   <a href="{{base_path}}/assets/img/get-started/kola-icon.png"><img src="{{base_path}}/assets/img/get-started/kola-icon.png" alt="Kola Icon" width="70%"></a>
2. Click on the **`Set Up Kola`** button.
3. The setup wizard will install and configure the [Ballerina](https://ballerina.io/) distribution required for Kola.
4. Click on the **`Restart VSCode`** button to complete the setup.
   <a href="{{base_path}}/assets/img/get-started/kola-setup.gif"><img src="{{base_path}}/assets/img/get-started/kola-setup.gif" alt="Kola Setup" width="70%"></a>

### Step 5: Create a new integration project.
1. Click on the Kola Integrator icon on the sidebar.
2. Click on the **`Create New Integration`** button.
3. Enter the Integration Name as `HelloWorld`.
4. Select Project Directory by clicking on the **`Select Location`** button.
5. Click on the **`Create New Integration`** button to create the integration project.
   <a href="{{base_path}}/assets/img/get-started/create-integration.gif"><img src="{{base_path}}/assets/img/get-started/create-integration.gif" alt="Create Integration" width="70%"></a>

### Step 6: Create an Integration Service.
1. In the design view, click on the **`Add Construct`** button.
2. Select **`Service`** from the menu.
3. Select **`HTTP Service`** from the Service Type dropdown.
4. Select **`Design From Scratch`** option. 
5. Enter the service name as `HelloWorldService`, path as `/hello`, and `9090` as the port.
6. Click on the **`Create Service`** button to create the new service with the specified configurations.
   <a href="{{base_path}}/assets/img/get-started/create-service.gif"><img src="{{base_path}}/assets/img/get-started/create-service.gif" alt="Create Service" width="70%"></a>

### Step 7: Design the Integration.
1. Now that you have created the service, you can design the integration by adding resources and methods to it. The generated service will have a default resource named `greeting` with a `GET` method.
2. Click on the `greeting` resource to view the resource details. Let's modify the resource to invoke the [`HelloWorld`](https://apis.wso2.com/zvdz/mi-qsg/v1.0) API endpoint.
3. Hover to the arrow after start and click the ➕ button to add a new action to the resource.
4. Select **`Add Connection`** from the node panel on the left. 
5. Select **`HTTP Connection`** as the connection type.
6. Change the variable name to `externalEP`.
7. Add the URL `https://apis.wso2.com` to the connection URL field and click **`Save`**.
   <a href="{{base_path}}/assets/img/get-started/create-connection.gif"><img src="{{base_path}}/assets/img/get-started/create-connection.gif" alt="Create New Connection" width="70%"></a>

8. Click the ➕ button again and select **`Connections`->`externalEP`->`Get`** from the node panel.
9. Enter the path `/zvdz/mi-qsg/v1.0` in the URL field and click **`Save`**.
   <a href="{{base_path}}/assets/img/get-started/add-action.gif"><img src="{{base_path}}/assets/img/get-started/add-action.gif" alt="Add Action" width="70%"></a>

10. Click on the ➕ button again and select **`Return`** from the node panel.
11. Select the `value` variable from the dropdown and click **`Save`**. This step will return the response from the `HelloWorld` API endpoint.
   <a href="{{base_path}}/assets/img/get-started/add-return.gif"><img src="{{base_path}}/assets/img/get-started/add-return.gif" alt="Add Return" width="70%"></a>

### Step 8: Run the Integration.
1. Click on the **`Run`** button at top right corner to run the integration.
2. The integration will be compiled and started in the embedded Ballerina runtime.
3. Once the integration is started, you can access the service by navigating to `http://localhost:9090/hello/greeting` in your web browser.
   