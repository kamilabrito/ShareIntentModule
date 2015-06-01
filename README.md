# ShareIntentModule
This is a simple android module to simplify the use of share intent.

# How to use
 - Import project as a module to your Android Project
 - Declare a ShareIntent variable in your Activity 
<p> <code> private ShareIntent shareIntent; </code>
 - Initialize variable with the instance of the ImageView that contain the image you want to share and your Activity's context <p> <code> shareIntent = new ShareIntent(image, getApplicationContext()); </code>
 - Call the intent from the trigger of your choice (button, action, broadcast...)
 <p> <code> startActivity(Intent.createChooser(shareIntent.shareImage(), "share via..."));</code>
