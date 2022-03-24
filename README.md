# stripe-test

[![Moove It](https://circleci.com/gh/moove-it/react-native-template.svg?style=svg)](https://app.circleci.com/pipelines/github/moove-it/react-native-template?branch=master)

This project is a test of stripe for react native. We simply implemented a `<TextInput />` on line 37 of `App.tsx` and then we get the next error:

```
E/unknown:ReactNative: Exception in native call
    java.lang.NullPointerException: Attempt to invoke virtual method 'boolean com.facebook.react.uimanager.FabricViewStateManager.hasStateWrapper()' on a null object reference
        at com.facebook.react.views.textinput.ReactEditText.updateCachedSpannable(ReactEditText.java:981)
        at com.facebook.react.views.textinput.ReactEditText.access$300(ReactEditText.java:75)
        at com.facebook.react.views.textinput.ReactEditText$TextWatcherDelegator.onTextChanged(ReactEditText.java:1092)
        at android.widget.TextView.sendOnTextChanged(TextView.java:11785)
        at android.widget.TextView.setText(TextView.java:6965)
        at android.widget.TextView.setText(TextView.java:6761)
        at android.widget.EditText.setText(EditText.java:145)
        at android.widget.TextView.setText(TextView.java:6713)
        at android.widget.TextView.setEditableFactory(TextView.java:6670)
        at androidx.emoji2.viewsintegration.EmojiEditTextHelper$HelperInternal19.<init>(EmojiEditTextHelper.java:268)
        at androidx.emoji2.viewsintegration.EmojiEditTextHelper.<init>(EmojiEditTextHelper.java:109)
        at androidx.appcompat.widget.AppCompatEmojiEditTextHelper.<init>(AppCompatEmojiEditTextHelper.java:52)
        at androidx.appcompat.widget.AppCompatEditText.<init>(AppCompatEditText.java:110)
        at androidx.appcompat.widget.AppCompatEditText.<init>(AppCompatEditText.java:91)
        at androidx.appcompat.widget.AppCompatEditText.<init>(AppCompatEditText.java:87)
        at com.facebook.react.views.textinput.ReactEditText.<init>(ReactEditText.java:126)
        at com.facebook.react.views.textinput.ReactTextInputManager.createViewInstance(ReactTextInputManager.java:180)
        at com.facebook.react.views.textinput.ReactTextInputManager.createViewInstance(ReactTextInputManager.java:81)
        at com.facebook.react.uimanager.ViewManager.createViewInstance(ViewManager.java:139)
        at com.facebook.react.uimanager.ViewManager.createView(ViewManager.java:76)
        at com.facebook.react.uimanager.NativeViewHierarchyManager.createView(NativeViewHierarchyManager.java:281)
        at com.facebook.react.uimanager.UIViewOperationQueue$CreateViewOperation.execute(UIViewOperationQueue.java:194)
        at com.facebook.react.uimanager.UIViewOperationQueue$DispatchUIFrameCallback.dispatchPendingNonBatchedOperations(UIViewOperationQueue.java:1110)
        at com.facebook.react.uimanager.UIViewOperationQueue$DispatchUIFrameCallback.doFrameGuarded(UIViewOperationQueue.java:1081)
        at com.facebook.react.uimanager.GuardedFrameCallback.doFrame(GuardedFrameCallback.java:29)
        at com.facebook.react.modules.core.ReactChoreographer$ReactChoreographerDispatcher.doFrame(ReactChoreographer.java:175)
        at com.facebook.react.modules.core.ChoreographerCompat$FrameCallback$1.doFrame(ChoreographerCompat.java:85)
        at android.view.Choreographer$CallbackRecord.run(Choreographer.java:1008)
        at android.view.Choreographer.doCallbacks(Choreographer.java:809)
        at android.view.Choreographer.doFrame(Choreographer.java:740)
        at android.view.Choreographer$FrameDisplayEventReceiver.run(Choreographer.java:995)
        at android.os.Handler.handleCallback(Handler.java:938)
        at android.os.Handler.dispatchMessage(Handler.java:99)
        at android.os.Looper.loop(Looper.java:246)
        at android.app.ActivityThread.main(ActivityThread.java:8653)
        at java.lang.reflect.Method.invoke(Native Method)
        at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:602)
        at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1130)
```

## Base dependencies

- [stripe](https://github.com/stripe/stripe-react-native).

### Using scripts from console

`yarn ios` or `yarn android`


## Screens
![image](https://user-images.githubusercontent.com/32213336/159972146-aa5da0d5-0fe4-42a2-80f5-ba8bdd06f955.png)

