## Using Azure AD B2C as an identity provider in Power Pages

Hi there, in my last article, I did a brief rundown of **Microsoft Power Pages**, you can check out the article [Quick Overview of Microsoft Power Pages](https://thecompletehub.tech/quick-overview-of-microsoft-power-pages). 

This same article was republished on **Microsoft Tech Blog** and now has over 1000 readers. You can also check it out - [Power Pages - Building Without Boundaries](https://techcommunity.microsoft.com/t5/educator-developer-blog/power-pages-building-without-boundaries/ba-p/3516041).

In this article, we will be taking a detailed breakdown of how to use **Microsoft Azure AD B2C as an identity provider in Power Pages, for setting up authentication**.

Let's get right into it!

# What is Azure AD B2C?

Azure Active Directory Business-to-Customer (Azure AD B2C) is an identity management service of Microsoft Azure that enables custom control of how your customers sign up, sign in, and manage their profiles when using your iOS, Android, .NET, single-page (SPA), and other applications.

Azure AD B2C is a separate service from Azure Active Directory (Azure AD). It is built on the same technology as Azure AD but for a different purpose.

Azure AD B2C provides a highly customizable **User Experience** to suit and blend with your brand seamlessly. Allowing you to customize every page when a user signs up, signs in, and modifies their profile information, providing a native look and feel that follows your web, mobile, and other applications. 

Check out the docs for more information [Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/).

## Using Azure AD B2C in Power Pages
Power Pages supports authentication processes and provides various authentication providers to handle authentication. 


![Screenshot 2022-07-12 at 19.41.53.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657651546255/11Q3FMgDf.png align="left")
With this, you can provide and set up several authentication providers on your website. 

Now, let us see how to set up Azure AD B2C to handle our authentication needs for our websites while building with **Microsoft Power Pages**.

**Requirements**

1. To duly follow this tutorial you need to have an Azure account and an active subscription plan

2. Before you can use the Azure AD B2C for authentication, they must be registered in a tenant that you manage.

3. Also, you need to have Microsoft.AzureActiveDirectory as a resource provider for the Azure subscription you're using. 

Follow this tutorial, to **[Create an Azure Active Directory B2C tenant](https://docs.microsoft.com/en-us/azure/active-directory-b2c/tutorial-create-tenant)**

If you followed the tutorial carefully, you should have successfully created your Azure Active Directory B2C tenant. 

**Next Step:**
The next step for setting up Azure AD B2C authentication for Power Pages is to **Register a web application in Azure Active Directory B2C**. 

Kindly follow this tutorial: **[Register a web application in Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/tutorial-register-applications?tabs=app-reg-ga)**

If you successfully followed the docs properly, you should have your web application registered in Azure Active Directory B2C.

Following the screenshot below, you should have your registered web application:
![Screenshot 2022-07-15 at 00.00.39.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657839670006/FPVddK1M2.png align="left")

The next thing to do is to **set up user flows and custom policies**. 
Let us follow this tutorial/documentation: [Create User flows and custom policies in Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/tutorial-create-user-flows?pivots=b2c-user-flow)

After following the previous tutorial in the link above, **(kindly get back to it, before you proceed with this step)**, let us head back to Identity Configuration Page in Power Pages, to complete our Configuration settings.

![Main.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657842228366/z3APN-v_L.png align="left")

**A few things to note, while configuring your Identity Configuration page in Power Pages: 
**
1. Authority: This is the issuer URL defined in the metadata of the sign-up & sign-in policy user flow 
![download.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657842681698/htdAL6Oc2.png align="left")

2. Client ID: The ID associated with the application created in Azure Active Directory B2C tenant to be used with the portal. 
![download (1).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657843099050/odu1y60UV.png align="left")

3. Redirect URL: This is the location where Azure AD B2C will send an authentication response. Enter the portal URL. You only need to change the redirect URI if you're using a custom domain name.

Kindly follow this tutorial/documentation to complete the Configuration settings on Power Pages: [Configure the Azure Active Directory B2C provider manually](https://docs.microsoft.com/en-us/power-apps/maker/portals/configure/configure-azure-ad-b2c-provider-manual?WT.mc_id=ppac_inproduct_resources).

Hit the confirm button to save and apply the settings applied. 

![Screenshot 2022-07-15 at 01.03.20.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1657843456855/BwuTd6Jpn.png align="left")

Now test your application. 

Congratulations you have successfully set up and configured Azure AD B2C in Microsoft Power Pages. 

# Announcement

I am building a community of Power Platform enthusiasts/developers, if you are interested, especially if you are in Ado-Ekiti, Ekiti State Nigeria, then please join us [Power Platform User Group Ado-Ekiti](https://powerusers.microsoft.com/t5/Power-Platform-User-Group-Ado/gh-p/PowerPlatformUserGroupAdo-Ekiti). 

The first annual Power Platform Conference sponsored by Microsoft and Power Platform Conference is coming to Orlando for an amazing in-person event on September 18-22.  Join us for special keynotes, sessions, breakouts, and more—all dedicated to Microsoft Power Platform products: Power Automate, Power Apps, Power BI, Power Pages, and Power Virtual Agents, register for this with my unique code:  **MPPCADEKUG** [Microsoft Power Platform Conference](https://powerplatformconf.com/#!/)

![MPPCADEKUG.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1657844367595/GLAGTkbIo.jpg align="left")

Kindly follow me on Twitter and make a Tweet, tagging me, if you learned something in this article. 
[Twitter](https://twitter.com/favour_adeshina)

Lastly, kindly subscribe to my newsletter and await my first exciting newsletter for all my subscribers. 

Thank You