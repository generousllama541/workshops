---
uid: Workshop.TubePlayer.Finalization
---

# Module 11 - Finalization

In this, you will finalize the app but adding extra bits and cleaning up the code.

## App navigation bar

1. Right-click the following image and save it in the  *Assets* folder.

    ![TubePlayer app navigation bar icon](navigation_bar.svg)

1. In *MainPage.cs* replace the sample image with as follows:

    ```csharp
    -.Source(new BitmapImage(new Uri("https://picsum.photos/384/40")))
    +.Source(new BitmapImage(new Uri("ms-appx:///TubePlayer/Assets/navigation_bar.png")))
    ```

    The reason for using the *png* extension is that the image gets internally translated to PNG format (see [Get started with Uno.Resizetizer](xref:Uno.Resizetizer.GettingStarted#how-it-works)).

## Import the TubePlayer splash screen

Right-click the following image and save it in the *TubePlayer.Base* project. Under the *Splash* folder, override the existing *splash_screen.svg* file with it.

![TubePlayer splash screen](splash_screen.svg)

## Import the TubePlayer app icon

Right-click the following image and save it in the *TubePlayer.Base* project. Under the *Icons* folder, override the existing *icon_foreground.svg* image with it.

![TubePlayer app icon](icon_foreground.svg)

This image is slightly different than the splash screen, as it is oriented to be displayed properly in the app drawer icon.

## Run the app

When you run the app, the app icon and the splash screen, as well as the navigation bar banner will appear on the screen.

![App icon, splash screen, and navigation bar are rendered](ui-output.gif)

---

**[Previous](xref:Workshop.TubePlayer.MediaPlayer "Add a media player")**