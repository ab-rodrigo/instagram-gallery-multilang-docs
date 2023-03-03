## Instagram Gallery Multi-language - OpenCart v3.x (OCMOD)

![Badge](https://img.shields.io/badge/oc_version-3.x-informational?style=flat&logoColor=white)
![Badge](https://img.shields.io/badge/ocmod-true-informational?style=flat&logoColor=white)
[![Badge](https://img.shields.io/badge/donate--brightgreen?style=flat&logoColor=white&logo=paypal)](https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW)

#### [Module page](https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=44728&filter_member=Rodrigoabr)

- [Welcome](#welcome)
- [Overview](#overview)
- [Resources](#resources)
- [Prerequisite](#prerequisite)
- [Upload files](#upload-files)
- [Install the module](#install-the-module)
- [Galleries](#galleries)
  - [Create a Main Gallery](#create-a-main-gallery)
  - [Create a Clone Gallery](#create-a-clone-gallery)
- [API configuration (Main Galleries only)](#api-configuration-main-galleries-only)
  - [Create a Facebook App](#create-a-facebook-app)
  - [Instagram Basic Display and API Configuration Module](#instagram-basic-display-and-api-configuration-module)
  - [Add an Instagram Test User](#add-an-instagram-test-user)
  - [Authenticate the User](#authenticate-the-user)
- [General configuration tab](#general-configuration-tab)
- [View configuration tab](#view-configuration-tab)
- [Display the gallery in the layout.](#display-the-gallery-in-the-layout)
- [Access and Modification Permissions](#access-and-modification-permissions)
- [Uninstall](#uninstall)
- [Troubleshooting](#troubleshooting)
- [Licence](#licence)
- [How to get help](#how-to-get-help)
- [Contact](#contact)
- [Buy me a coffee](#buy-me-a-coffee)

# Welcome
Welcome to the documentation for the Instagram Gallery Multi-Language module for Opencart versions 3.x.

# Overview
Display your Instagram posts directly on your store with ease. Utilize Meta's official API to showcase your Instagram posts as an image gallery on your online store. Create a variety of visualizations, add effects, titles, subtitles, links to the original media post, navigation buttons, pagination buttons, and much more. Configure the API once and create multiple galleries, each with a unique visualization style, and display them in different layouts.
<p align="center"><img src="images/overview.png" alt="Overview" title="Overview"></p>

# Resources
+ 3 types of visualization
+ Title
+ Caption
+ Pagination
+ Link to original Instagram post
+ Image Effects
+ Clone gallery (Multiple galleries with a single API)
+ Available in
   - English (en-gb)
   - Portuguese (pt-br)

# Prerequisite
+ OpenCart v3.x installed as public website with SSL certificate (**SSL certificate is required for API integration**.).
+ A <a href="https://developers.facebook.com/" target="_blank">Facebook Developer Account</a>.
+ An <a href="https://www.instagram.com/" target="_blank">Instagram account</a>.
+ The user must have the following access and modification permissions:
  - *Dashboard > Extensions > Installer*
  - *Dashboard > Extensions > Extensions*
  - *Dashboard > Extensions > Modifications*
  - *Dashboard > Design > Layout*

To grant or revoke permissions, refer to the [Access and Modification Permissions](#access-and-modification-permissions) section.

# Upload files
Go to **_Extensions_ > _Installer_**. In the form that appears, click on the **_Upload_** button.
<p align="center"><img src="images/upload_file.png" width="600" alt="Upload files" title="Upload files"></p>

Please locate the previously downloaded file **instagra_gallery_multilang_3.x.ocmod.zip**, select it, and click on the **_Open_** button or double-click on the file name.

<p align="center"><img src="images/select_instalation_file.png" width="600" alt="Select instalation file" title="Select instalation file"></p>

Please wait for the installation to finish, then the module will be listed in the **_Install History_** table.

Go to **_Extensions_ > _Modifications_** and click on the **_Refresh_** button.
<p align="center"><img src="images/refresh_modifications.png" width="600" alt="Refresh modifications" title="Refresh modifications"></p>

# Install the module
Go to **_Extensions_ > _Extensions_**, select **_Modules_** from the dropdown menu, locate the **_Instagram Gallery Multilang_**, and then click on the **_Install_** button at the end of the line.
<p align="center"><img src="images/install_module.png" width="600" alt="Install the module" title="Install the module"></p>

# Galleries
About gallery types
>There are two ways to create a gallery:
>1. [_Main Gallery_ or _Parent Gallery_](#create-a-main-gallery): This type of gallery will contain the Instagram API configuration. Multiple Main Galleries can be created, each with a different API configuration.
>2. [_Clone Gallery_ or _Child Gallery_](#create-a-clone-gallery): This type of gallery will use the API settings of the Main Gallery. Multiple Clone Galleries can also be created for each Main Gallery.

## Create a Main Gallery
Go to **_Extensions_ > _Extensions_**, select **_Modules_** from the drop-down menu, locate the **_Instagram Gallery Multilang_**, and then click on the **_Edit_** button at the end of the line.
<p align="center"><img src="images/add_gallery.png" width="600" alt="Add gallery" title="Add gallery"></p>

Enter the name of the _new gallery_ and click on the Save button. The name of the gallery can be changed later.
<p align="center"><img src="images/add_gallery_name.png" width="600" alt="Add gallery" title="Add gallery"></p>

## Create a Clone Gallery
Go to **_Extensions_ > _Extensions_**, select **_Modules_** from the select menu, locate the **_Instagram Gallery Multilang_** then click on the **_Edit_** button at the end of the line.        
<p align="center"><img src="images/add_gallery.png" width="600" alt="Add clone gallery" title="Add clone gallery"></p>

Enter the name of the new _child gallery_, select the _parent gallery_ and click the Save button. The name of the gallery can be changed later.
<p align="center"><img src="images/add_clone_gallery_name.png" width="600" alt="Add clone gallery name" title="Add clone gallery name"></p>

# API configuration (Main Galleries only)
This chapter/tutorial demonstrates how to configure an Instagram App in the app dashboard and how to set up the API for the module.
>Before you start, make sure you already have a <a href="https://developers.facebook.com/" target="_blank">Facebook Developer Account</a>  and the store is not in maintenance mode.
<!-- <p align="center"><img src="images/api_tab_form.png" width="600" alt="API configuration" title="API configuration"></p> -->

## Create a Facebook App
Go to <a href="https://developers.facebook.com/" target="_blank">Facebook Developer Account</a>, click **_My Apps_**, and create a new app.
<p align="center"><img src="images/my_apps_empty.png" width="600" alt="My apps" title="My apps"></p>

Choose the **_Consumer_** or **_None_** app type.
<p align="center"><img src="images/app_type.png" width="400" alt="App type" title="App type"></p>

Add an app name.
<p align="center"><img src="images/add_app_name.png" width="600" alt="Add app name" title="Add app name"></p>

After creating the app, go to the App Dashboard, navigate to **_Settings > Basic_**, scroll to the bottom of page, and click **_Add Platform_**.
<p align="center"><img src="images/add_plataform.png" width="600" alt="Add plataform" title="Add plataform"></p>

Choose **_Website_** and click **_Next_**.
<p align="center"><img src="images/select_plataform.png" width="400" alt="Select plataform type" title="Select plataform type"></p>

Add your website’s URL, and save your changes.
><img src="images/copy_button.png" width="50" alt="Copy button" title="Copy button">
>Click on this button to copy the store's URL.
<p align="center"><img src="images/copy_paste_website_url.png" width="600" alt="Add website's URL" title="Add website's URL"></p>

## Instagram Basic Display and API Configuration Module
Click on **_Products_**, locate the **_Instagram Basic Display_** product, and click **_Set Up_** to add it to your app.
<p align="center"><img src="images/instagram_basic_display_setup.png" width="600" alt="Instagram basic display setup" title="Instagram basic display setup"></p>

Scroll to the bottom of the page and click **_Create New App_**.
<p align="center"><img src="images/create_new_app.png" width="600" alt="Instagram basic display setup" title="Instagram basic display setup"></p>

Enter the name of the Facebook app that you just created.
<p align="center"><img src="images/create_a_new_instagram_app_id.png" width="600" alt="Create a new Instagram App ID" title="Create a new Instagram App ID"></p>

Please go back to the API tab of the module, copy the store URL, and paste it into the **_Valid OAuth Redirect URIs_**, **_Deauthorize callback URL_** and **_Data Deletion Request URL_**, then click 'Save.
<p align="center"><img src="images/copy_paste_oauth_uri.png" width="600" alt="Copy and paste OAuth URI" title="Copy and paste OAuth URI"></p>

In the Instagram Basic Display form, copy the **_Instagram App ID_** and **_Instagram App Secret_** numbers and paste them in the API tab of the module.
<p align="center"><img src="images/copy_paste_instagram_ids.png" width="600" alt="Copy and paste Instagram App ID" title="Copy and paste Instagram App ID"></p>

## Add an Instagram Test User
Please navigate to **_Roles > Roles_** and scroll down to the **_Add Instagram Testers_** section. Then, click **_Add Instagram Testers_** and enter your Instagram account's username before sending the invitation.
<p align="center"><img src="images/add_instagram_test_user.png" width="600" alt="Add Instagram user test" title="Add Instagram user test"></p>

Open a new web browser and go to instagram.com. Sign into your recently invited Instagram account. Navigate to **_(Profile Icon) > Edit Profile > Apps and Websites > Tester Invites_**, and accept the invitation
<p align="center"><img src="images/tester_invites.png" width="600" alt="Tester invites" title="Tester invites"></p>

Your Instagram account is now eligible to be accessed through your Facebook app.

## Authenticate the User
Go to the API tab of the module and click on the **_Authorization_** button.
<p align="center"><img src="images/authorization_button.png" width="600" alt="Authorization button" title="Authorization button"></p>

Click the **_Open Authorization Window_** button or copy and paste the link into your browser. It is necessary to be logged into the Instagram account that will provide the media for the gallery.
<p align="center"><img src="images/authorization_popup.png" width="400" alt="Authorization popup" title="Authorization popup"></p>

The authorization window should appear and display your Instagram username, the name of the app, and a description of the permissions it is requesting. Click **_Authorize_** to grant the app access to your profile data.
<p align="center"><img src="images/authorization_window.png" width="250" alt="Authorization window" title="Authorization window"></p>

Please access the module page and refresh it. Then, go to the API tab and verify that the API status displays the correct configured API message.
<p align="center"><img src="images/api_status_success.png" width="600" alt="Api success" title="Api success"></p>

The setup for Instagram Basic Display and Module API is complete when the API status displays the correct configured API message. Set the General and View settings, and click the 'Save' button at the top of the page to create your gallery.

# General configuration tab
<p align="center"><img src="images/general_tab_form.png" width="600" alt="General configuration" title="General configuration"></p>

+ **Name**: This text is used to identify the gallery. Duplicate names for galleries are not permitted.
+ **Title**: The title that will be displayed above the gallery allows you to use HTML and CSS.
+ **Types of posts**: Types of Instagram posts that will provide content for the gallery.
+ **Album media type**: Types of media that will be provided from the albums.
+ **Images from album**: The quantity of media that will be provided from the albums.
+ **Update**: Period during which the oldest image in the gallery will be updated.
+ **Status**: Gallery status.

# View configuration tab
<p align="center"><img src="images/view_tab.png" width="600" alt="View configuration" title="View configuration"></p>

+ **Media per view**: The maximum number of media that will be displayed.
+ **View type**: Type of visualization.
+ **Pagination**: Show pagination bullet points.
+ **Zoom effect**: Type of zoom effect while mouse hovers over the image.
+ **Rounded edges**: Apply rounded edges to the images.
+ **Skew**: Apply a tilt effect to the image.
+ **Color effect**: Type of color effect when the mouse hovers over the image.
+ **Caption**: Display part of the post caption.
+ **Link original post**: Access the original posts by clicking on the images.
+ **Mobile**: Display the gallery on devices with a screen resolution of less than 576px.

# Display the gallery in the layout.
Go to **_Design_ > _Layouts_**, find the layout where you want to display the gallery, and click **_Edit_** at the end of the row.
<p align="center"><img src="images/layout_list.png" width="600" alt="Layout list" title="Layout list"></p>

Choose the position in which the gallery will be displayed. In the drop-down menu, locate the gallery by name, click the **_Add Module_** button, and save the changes.
In this example, we will configure the gallery to be displayed at the Content Bottom.
<p align="center"><img src="images/layout_form.png" width="600" alt="Layout form" title="Layout form"></p>

# Access and Modification Permissions
Go to **System > Users > Users Groups**, locate your group by name, and click **_Edit_** at the end of the row.

In the **_Access Permissions_** and **_Modification Permissions_** lists, find the line **_extension/module/instagram_gallery_multilang_** and make sure it is checked.
<p align="center"><img src="images/permissions.png" width="600" alt="Permissions" title="Permissions"></p>

# Uninstall
<p align="center">
<img src="images/caution.png" width="400" alt="Permissions" title="Permissions"></p>
When uninstalling the module, all settings, galleries, and media will be deleted. 

Go to **_Extensions > Installer_**, locate the module, and click **_Uninstall_** at the end of the row.
<p align="center"><img src="images/uninstall.png" width="600" alt="Uninstall" title="Uninstall"></p>

# Troubleshooting
Access the <a href="https://github.com/ab-rodrigo/instagram-gallery-multilang-docs/blob/main/troubleshooting.md" target="_blank">Troubleshooting</a>.  page.

# Licence
GNU General Public License version 3 (GPLv3) - https://www.gnu.org/

# How to get help
[Module page](https://www.opencart.com/index.php?route=marketplace/extension/info&extension_id=44728&filter_member=Rodrigoabr)

Please access the module page and click on the 'Get Support' button.

# Contact
Rodrigo Barbosa - ab.rodrigo@outlook.com

# Buy me a coffee
<p align="center"><a href="https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW" target="_blank"><img src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" alt="Donate with PayPal button" title="PayPal - The safer, easier way to pay online!"></a></p>
