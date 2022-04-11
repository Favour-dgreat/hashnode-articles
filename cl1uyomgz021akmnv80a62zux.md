## Getting Started with Microsoft Power Apps - Building a Simple Canvas App

Welcome to the third article of the [Microsoft Power Platform Series](https://thecompletehub.tech/series/power-platform) in the previous article we learned how to use Data connectors while building applications with Microsoft Power Apps - [Check it out](https://thecompletehub.tech/understanding-data-connectors-with-microsoft-power-apps).

In today's article, we will be building a simple Canvas App, for you to be reading this you should be familiar already with what Canvas Apps are from my previous article. Feel free to go through the article in other to understand better what will be discussed here. [Microsoft's Power Platform - Low Code Platform ](https://thecompletehub.tech/microsofts-power-platform-lowcode-platform). 

Let's start!

# Setting up your Microsoft 365 Developer Account 
A Microsoft 365 account pulls together all the traditional Office apps, such as MS Word, Excel, PowerPoint, etc., so having a Microsoft 365 Developer account will provide access to these apps. 


![Screenshot 2022-04-08 at 12.25.36.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649417144937/6WQTE0RPD.png)

You should also know that your Microsoft's Power Platform products (Power Apps, Power Automate, Power BI, and Power Virtual Agents) are all included in Office Apps, so in order to have access to these apps for building you need to have a Microsoft 365 Account. 

Following these steps, we are going to join the Microsoft 365 Developer Program:


1. Visit this link [Microsoft 365 Developer Center](https://developer.microsoft.com/en-us/microsoft-365/dev-program)

2. Click on Join now

3. Enter your Microsoft account registered email address and then complete the authentication process

![Screenshot 2022-04-08 at 12.39.16.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649422778993/j0CVKP8re.png)


*If you do not know what a Microsoft account is, or need help setting up one then please read this article * [How to create a new Microsoft account](https://support.microsoft.com/en-us/account-billing/how-to-create-a-new-microsoft-account-a84675c3-3e9e-17cf-2911-3d56b15c0aaf)

If you followed through the authentication process you will have this screen. 
![Screenshot 2022-04-08 at 14.26.23.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649424391193/IoJkZulaZ.png)


4.Click on the Button Setup E5 Subscription, and then click on instant sandbox 
![Screenshot 2022-04-08 at 14.31.27.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649424907430/SggbKe1PZ.png)

5.Add a valid Phone Number for security and then get your verification code
![Screenshot 2022-04-08 at 14.31.53.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649425128391/vdy6DbJhr.png)

6.And then you successfully have your E5 Subscription, which will allow you premium access to Office Applications for the next 90 days.   

![Screenshot 2022-04-08 at 14.32.33.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649425279700/lYnUHQwYa.png) 

**Note: This subscription is available for free for just 90 days after which you will need to pay for it, but by joining the Microsoft Learn Student Ambassador program, you have access to all Office applications for free, throughout your ambassadorship period. This and other amazing benefits include subscriptions for various Microsoft Certification exams, to know more and become a [Microsoft Learn Student Ambassador](https://studentambassadors.microsoft.com/)
**

# Building a Canvas App

Now that we now have a subscription to access Office Applications, including our Power Platform products, we can now dive into [PowerApps](https://www.powerapps.com/) to start building our Canvas App.

Sign in with the email associated with the E5 Subscription

![Screenshot 2022-04-08 at 20.51.43.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649447568937/630cJ-4_2.png)

After successfully signing in to Power Apps, click on the Blank App card:
![Screenshot 2022-04-08 at 20.53.57.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649447708579/AR3gfy-zh.png)

Click the create button, for us to create a Blank canvas app:
![Screenshot 2022-04-08 at 20.54.36.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649447875342/vWU9d7x8-.png)

You then give the app a name and click on the Phone radio button option, for the app format

![Screenshot 2022-04-08 at 21.01.34.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649448210521/_4GXu5wAq.png)

You will be provided with a blank screen to start working on. 

![Screenshot 2022-04-08 at 21.06.59.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649448464319/kcgGBU1Zv.png)

On the right side, in the properties settings, change the fill color to any color of choice and add a background image 

![Screenshot 2022-04-08 at 21.11.37.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649448790397/9iBk6CK5H.png)

Click on the add button on the left side of the screen, let us add a text label to our app
 

![Screenshot 2022-04-08 at 21.18.27.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649449125284/PLSPk-oec.png)

Enter a text as your app label. On the right side of the screen, you have the option to adjust the properties of the text label. This includes changing the font size, alignment, color, font weight, etc., kindly check them out to add more beauty to your app. 


![Screenshot 2022-04-08 at 21.22.30.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649449366503/0Wf2eBEmP.png)

Now let us proceed to add a button to our app

Still, on the insert pane, scroll and locate the button as part of the insert tools/options and click on it. Then on the right side of the screen, add the button's text. Feel free to style the text more by checking out the other font options.  

![Screenshot 2022-04-08 at 21.27.08.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649449691355/5Jp7O52Ip.png)

With the last task, we are done with screen 1, let us proceed to screen 2. 

On the top menu, click on the New Screen button dropdown and select the tutorial Screen option

![Screenshot 2022-04-08 at 21.31.34.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649449963140/HwjqhyTpm.png)

A Tutorial Screen shows people how to use your app. 

![Screenshot 2022-04-08 at 21.38.19.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649450328283/JLLzUCfSH.png)

Click on the image placeholder on the screen and notice the code beside the function button


![Screenshot 2022-04-08 at 21.40.42.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649450589443/ijAUuXoeb.png)

Replace the code with this; 

```
If(IsBlank(_guideStep), First(TutorialNavigator1.AllItems).Text, LookUp(TutorialNavigator1.AllItems, Step = _guideStep).Text)
``` 
We changed the code to remove the image placeholder that comes with the tutorial screen as we won't be needing it for this app. 

Our screen now looks like this:

![Screenshot 2022-04-08 at 21.58.44.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649451548167/tGfNvxRoh.png)

Now let us add a background image and adjust the background and the fill color. 


![Screenshot 2022-04-08 at 22.00.13.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649451628738/l8wgG0355.png)

Now let us change the "Create a tutorial to show people how to use your app" text and other default text in the app. To do this click the TutorialNavigator1 Gallery tool.

![Screenshot 2022-04-08 at 22.10.04.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649452323094/ON0Dp0hUQ.png)


Now let us edit the text for Step:0 to Step:3. Just copy and paste the code we have below to replace the default text.

```
Table(           
 {Step: 0, Text:"Welcome"},           
 {Step: 1, Text:"Add an Event"},           
 {Step: 2, Text:"Save the event and view on next screen"},           
 {Step: 3, Text:"Edit or Delete an already exisiting event"}
 
)
``` 

Now you can go ahead to format the text using the font properties we have on the right side of the screen, just like I have done here. 

![Screenshot 2022-04-08 at 22.18.21.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649452770302/IEp4q0-JV.png)

Now click the Skip text button, adjust the font size and color, and then on the right side of the screen, click on the advanced, and then under the action, under the onSelect paste the code below: 

```
Navigate(Screen3, ScreenTransition.Fade)
``` 

![Screenshot 2022-04-08 at 22.30.57.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649453477606/rgpz7ucJ4.png)

**Note: This will bring up some form of error and this is because in our formula we introduced Screen3, which we don't have yet in our app. Let us quickly dive into adding Screen3 to remove this error and proceed with our app. 
**
As we did earlier while creating our Screen2 click on the New Screen Button dropdown in the top menu and select the Screen with confirmation text screen option

![Screenshot 2022-04-08 at 22.33.14.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649453673869/5MtbyrRhh.png)

Adding the third screen automatically removes the error faced earlier with the formula added to the skip textButton in Screen2

![Screenshot 2022-04-08 at 22.34.56.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649453770798/5s7mHpvbo.png)

Now let us continue with editing our Screen3, this is what your Screen3 should look like: 

![Screenshot 2022-04-08 at 22.37.52.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649453878447/4liLaHDPl.png)

The first thing to do is to add a background image and the fill color, then replace the custom text with this: "Congratulations! You are now ready to use this app" and format the text as you want, just as I have done here. 

![Screenshot 2022-04-08 at 22.42.37.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649454164422/w383Nai7P.png)
 
Finally, for Screen3 we are going to add an icon that onClicked will take us to the next screen.
On the insert pane, locate the Icons tool and search for "next arrow", then click on the search result to add the icon to Screen3. 

![Screenshot 2022-04-08 at 22.48.24.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649454522114/MWdmLP05F.png)

Drag down the icon added to be immediately under the text added earlier. Also, let us add an action for the icon to perform when clicked. Just like we added an action for the skip textButton in Screen2, we are going to be doing the same thing here. Copy and past the code below: 


```
Navigate(Screen4, ScreenTransition.Fade)
``` 

![Screenshot 2022-04-08 at 23.10.33.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649455839170/y9NmBpqwa.png)

The code above is simply to Navigate to Screen 4 in our app with a fade transition, its quite straightforward. 

Now we are facing the same issue faced earlier and we will resolve it by adding a new Screen to our app. 

Moving forward now to add a New screen to our app. Click on the New Screen Button dropdown in the top menu and select the List screen. This is what your new screen should look like

![Screenshot 2022-04-08 at 23.18.04.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649456312773/XPlKTbnA-.png)

Now we are going to be making use of our Data connectors to connect to a Data Source, if you want to know more about Data Connectors, kindly check out my previous article [Understanding Data Connectors with Microsoft Power Apps](https://thecompletehub.tech/understanding-data-connectors-with-microsoft-power-apps) 

Click on the BrowseGallery tool in Screen4 to select a data source

![Screenshot 2022-04-08 at 23.22.32.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649456670623/fqtikmCfh.png)

However, right now we have no table or connector in our current environment. *(some links in the previous article will explain more on connectors and environments in power apps)*. We are going to fix that right now: 

1. Click the back arrow on the top menu back to return to the home screen

![Screenshot 2022-04-09 at 16.05.13.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649516923979/azBs8KiBB.png)
2. Click on connections, to add a new connection to the app. 

In this app, for my data source, I will be using an already created Google sheet.
So I will connect to Google Sheets, by signing into my Gmail and then authorizing Power Apps to have access to my Google Account.  

After everything is done, this is what I have: 

![Screenshot 2022-04-09 at 16.15.29.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649517335983/tLo_ZkbfS.png)

Now let us return back to building our app, by heading back to Screen 4 and connecting to an already existing Google Sheet in our connected Google Account.  

![Screenshot 2022-04-10 at 21.58.54.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649624369113/hM9zcM1zJ.png)

Now after successfully connecting to an existing Google sheet, hence the following data was added to Screen4:
![Screenshot 2022-04-10 at 22.02.27.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649624553571/4ZRXmYJJD.png)

Lastly for Screen4, I will adjust the layout and the font style and also add a Button to Register a New event. 

After everything is done, this is the new look for Screen4: 

![Screenshot 2022-04-10 at 22.25.32.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649625939674/XCWK8114X.png)

Moving forward we are going to be adding a new screen. So kindly go through the process as done earlier. We are going to be adding a Form Screen as Screen5.

![Screenshot 2022-04-10 at 22.27.23.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649626091486/WqnHagfmH.png)

The next action is to Edit the Screen properties, add a Title and connect to a Data Source.

*You should be able to do this now, following our previous activities *

![Screenshot 2022-04-10 at 22.28.31.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649626117613/gZGS9XjbE.png)

![Screenshot 2022-04-10 at 22.28.21.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649626607687/4MDV_pVg2.png)

After connecting to your Data Source, the next step is to add fields in the form. 
But in this case, because we are connected to the data source, Power Apps provides the form as required in our Data Source. So we proceed by ticking the fields, in other to add them to the form.  

![Screenshot 2022-04-10 at 22.38.10.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649626711460/l2GTwkqeC.png)

After adding the forms to the field:
![Screenshot 2022-04-10 at 22.41.55.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649626946331/3WST9higc.png)

Add a Button and replace the action function, by pasting the code below;

```
SubmitForm(EditForm1)
``` 

![Screenshot 2022-04-10 at 22.47.30.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649627256586/jIn3XIslX.png)

We are done with Screen5, moving forward to Screen6. Our last screen for this tutorial app. 

Add a new screen, following the previous description. This screen is a Scrollable screen. 

To make the screen functional, kindly do the following: 
1. Add a form that is connected to our Google Sheet Data Form
2. Add Custom Cards as done earlier
3. Adjust the added Cards with the following advanced options, as seen in the image below: 

![Screenshot 2022-04-10 at 23.57.51.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649680170074/sTtQQ7X0O.png)

![Screenshot 2022-04-10 at 23.59.42.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649680204502/M8mL_wuJv.png)

Adjust the form advanced options, as seen in the image above

4. Add the icons seen below along with the title and the button 

![Screenshot 2022-04-11 at 14.10.31.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649682864199/fovi2v8vB.png)

Adjust the properties, for the icons and the button, following these images: 


![Screenshot 2022-04-11 at 14.38.02.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649684451543/cuaFV6NTr.png)

![Screenshot 2022-04-11 at 14.38.08.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649684485980/KwNiOOWz9.png)

![Screenshot 2022-04-11 at 14.42.42.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649684569524/19q67ZlPl.png)

![Screenshot 2022-04-11 at 17.16.59.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1649693864649/6bDu12axk.png)

If you followed duly you should have a functioning event recording app. 

%[https://youtube.com/shorts/sitW9uOeTvg?feature=share]

# Resources

1. [Overview of connectors for Canvas Apps ](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/connections-list)
2. [Use of custom connectors in a Power Apps Canvas Apps](https://docs.microsoft.com/en-us/learn/modules/use-custom-connectors-in-powerapps-canvas-app/)
3. [Use Custom connectors with the timeline control](https://docs.microsoft.com/en-us/powerapps/maker/model-driven-apps/custom-connectors-timeline-control)
4. [Create a canvas app from a template](https://docs.microsoft.com/en-us/power-apps/maker/canvas-apps/get-started-test-drive)
5. [Create a canvas app with data from an Excel file](https://docs.microsoft.com/en-us/power-apps/maker/canvas-apps/get-started-create-from-data)

So concluding now, a Youtube video will be released, still on this article, to better explain everything here. So, subscribe to our Youtube Channel [The Complete Hub](https://www.youtube.com/channel/UCqrjXe8zo2-F-QoQXlmVCYw) 

Also, remember to Subscribe to our newsletter, like and comment on this article, and finally please share.

Thank You.