# BrowserPlus Uploader

The BrowserPlus Uploader tool allows you to easily create an advanced uploader widget that supports native drag+drop from
the desktop, multiple file selection from the file browse dialog, multiple simultaneous uploads (3 files at a time), and
Zip file compression. Skinning is also possible with plenty of parameters that may be overridden to specify colors, fonts,
labels and borders. All of this is packaged into two Javascript files (browserplus-min.js and uploader-min.js) that weigh
in at a combined 20KB of minimized Javascript.

To use the upload tool:

Create and place a block type element like div on your webpage. Specify the height and width of the element:

    <div id="myUploader" style="width:600px; height:200px"></div> 

And include the base BrowserPlus library, and the advanced upload JavaScript library at the bottom of your webpage:

    <script src="http://bp.yahooapis.com/2.4.17/browserplus-min.js"></script>  
    <script src="http://bp.yahooapis.com/toolbox/uploader/1.0.6/uploader-min.js"></script>  

Create an instance of the Uploader tool and point it at your uploader element. The second argument contains configuration
parameters:

    var uploader = BPTool.Uploader.create("myUploader", { /* config params */});  
    uploader.render();

It's important to understand that this JavaScript library is a convenience wrapper around BrowserPlus services, and its
use is completely optional. Much more flexibility and control is available by directly using the BrowserPlus JavaScript
API.

The browserplus site has all of the 
[configuration details and screenshots](http://browserplus.yahoo.com/developer/web/toolbox/upload/).
