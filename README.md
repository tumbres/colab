# colab
Google Colab
Stop Google Colab From Disconnecting!
Just open your Chrome DevTools by pressing F12 or Ctrl+Shift+I on Linux and run the following JavaScript code in your console:

function KeepClicking(){
   console.log("Clicking");
   document.querySelector("colab-toolbar-button#connect").click()
}setInterval(KeepClicking,60000)

Here, the value 60,000 represents the milliseconds(equivalent to one minute). 
This small piece of code makes a click on the Colab screen after every 60 seconds. 
Thus, Colab thinks that the notebook is not idle and you don’t have to worry about being disconnected!
