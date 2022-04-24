## Using Timer Control in PowerApps

Hi there, in the previous article we built a Simple Event Management Canvas App and in today's article, we will be adding a timer control feature to our already existing app, while learning about using timer control in PowerApps. 

Check out the previous article in this series[Getting Started with Microsoft Power Apps - Building a Simple Canvas App](https://thecompletehub.tech/getting-started-with-microsoft-power-apps-building-a-simple-canvas-app) and let's get started!

# What is Timer Control in PowerApps?
Timer Control in PowerApps is simply an Input Component amongst the Insert tools used for building apps. 

![Screenshot 2022-04-23 at 23.20.40.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650752465275/HaJJ1AO--.png)

It's also a control that can determine how your app responds after a certain amount of time passes.
Timers can, for example, determine how long a control appears or change other properties of a control after a certain amount of time has passed.


# Key Properties for using Timer Control Component 

**Duration** – How long a timer runs in milliseconds. The maximum is 24 hours expressed in milliseconds. Default is 60 seconds.

**OnTimerEnd** – Actions to perform when a timer finishes running.

**Repeat** – Whether a timer automatically restarts when it finishes running.

**AutoPause** – Whether the timer control automatically pauses if the user navigates to a different screen.

**AutoStart** – Whether the timer control automatically starts to play when the user navigates to the screen that contains that control.

**OnSelect **– Used to set actions to perform when the user taps or clicks the Timer component.

**OnTimerStart** – User to set actions to perform when a timer starts to run.

With the above definitions of the concept of Timers and Timer Control in Power Apps, in the next section, we will actually use Timer Control to enhance our already built app in the previous article/learn series.

# Implementing Timer Control Component 
Remember what our app looked like after the last article/learn series, check out this video:

%[https://www.youtube.com/shorts/sitW9uOeTvg]

Now let us implement our Timer Control Component in our app: 

Go to Screen 3 (Our Success Screen)
![Screenshot 2022-04-23 at 23.36.24.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650753412047/8xDuLRr3X.png)

Click on the Insert Tool Item and Search for Timer
![Screenshot 2022-04-23 at 23.38.06.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650753546954/uo87lDPs4.png)

Add the Timer to Screen3 Components

![Screenshot 2022-04-23 at 23.40.03.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650753637767/XaTil-hWw.png)

Now, we need to set a few parameters of the Timer –
Duration, you can specify in milliseconds here. Example: 3000 i.e. 3 seconds
![Screenshot 2022-04-23 at 23.42.13.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650753746393/MRzZPk_pB.png)

Next, you’ll need to set the Start flag. By default, this is set to false. The Start is triggered when the value is set to True. This needs to be dynamically set from elsewhere i.e. in this example, you’ll need to trigger from where you come to this screen so that the Timer starts the countdown.

![Screenshot 2022-04-23 at 23.44.00.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650753870590/sEt69kDsO.png)

Now, the way I set this is, first I create a variable from the place where I want to trigger the Timer to go off, that is my previous Screen (Screen2).  I’m creating and setting a variable called startTimer and setting the value to true:

![Screenshot 2022-04-24 at 00.09.54.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650755420667/M5h7eltB1.png)

You will then return to your Timer Component in Screen3 and set this variable startTimer to the Start property.

![Screenshot 2022-04-23 at 23.53.36.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650754432720/q1AghZ4ve.png)

Also, you’ll need to set what needs to happen when the Timer ends. So, you have to write the OnTimerEnd property as to what will happen once the Timer ends.
Here, you’ll Navigate to the 'Screen4’ as per our scenario and then also, set the startTimer flag to ‘false’ since you want to reuse this again for the next submission.

Now this works fine as Screen 4 loads immediately after the duration of the timer is elapsed.

Finally, I will hide the timer component from showing on the screen. 
To do this I will set the visible property to false. It is set to true by default, and by doing this immediately our timer becomes not visible but still works properly. 


![Screenshot 2022-04-24 at 00.14.39.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650755803020/zV9xntL2b.png)


![Screenshot 2022-04-24 at 00.14.52.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650755832207/AivDtFZg9.png)

In conclusion, with this new feature added to our app, we can now remove the previous buttons added to navigate to Screen4 from the Success Screen (Screen3), and this is the new look for Screen 3

![Screenshot 2022-04-24 at 00.19.24.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1650755992913/aB_UqMDol.png)

Now we have improved our app by using the Timer control component to our app. 


As said earlier to fully understand everything discussed up till this point, kindly read the previous article. 

Also, a YouTube Video to explain the previous article along with this will be released soon, kindly subscribe to our YouTube Channel to be notified [The Complete Hub](https://www.youtube.com/channel/UCqrjXe8zo2-F-QoQXlmVCYw)

# Learning Resources

1. [Timer control in Power Apps](https://docs.microsoft.com/en-us/power-apps/maker/canvas-apps/controls/control-timer?WT.mc_id=DX-MVP-5003911)
2. [Formula reference for Power Apps](https://docs.microsoft.com/en-us/power-apps/maker/canvas-apps/formula-reference)
3. [Get started with formulas in canvas apps](https://docs.microsoft.com/en-us/power-apps/maker/canvas-apps/working-with-formulas)
4. [Controls and properties in canvas apps](https://docs.microsoft.com/en-us/power-apps/maker/canvas-apps/reference-properties)
5. [Power Apps Ideas (preview)](https://docs.microsoft.com/en-us/power-apps/maker/canvas-apps/power-apps-ideas)
6. [Microsoft's Power Platform - LowCode Platform](https://thecompletehub.tech/microsofts-power-platform-lowcode-platform)

# Announcement
By next month I will be creating a closed Telegram group for a Power Apps crash course, show interest by filling out this form:


[Join the waitlist](https://u1v5w5q6g6n.typeform.com/to/QAh0PRrh)