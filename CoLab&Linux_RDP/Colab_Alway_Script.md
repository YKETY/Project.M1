Press F12 Then Go Console And Paste This Code
----------
function ConnectButton(){  
    console.log("Connect pushed");   
    document.querySelector("#top-toolbar > colab-connect-button").shadowRoot.querySelector("#connect").click()   
}  
setInterval(ConnectButton,60000);  
