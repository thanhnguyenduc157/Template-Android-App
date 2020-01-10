# mvvm clean architecture - app


The sample demonstrates an alternative implementation of the mvp-app sample using the [Model-View-ViewModel](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93viewmodel)(MVVM) architecture and Clean Architecture


### What you need

Before exploring this sample, you might find it useful to familiarize yourself with the following topics:

-   The  [MVVM](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93viewmodel)  architecture


Inputs is a set of actions and events that have impacts on viewModel such as the tap action on a button, or the viewDidLoad event. 

Outputs represents changes that views should reflect. Since ouputs may change over time, it’s best to return an Observable for each ouput. Behaviors defined in inputs should not be expressed as Variable because we don’t need the inputs to be obseravable.

And in this project we use Clean Architecture



### Implementing the app

Each version of the app implements the same features using a different approach to showcase and contrast a variety of architectural designs. For example, this version takes the following approaches to solving common implementation questions:

-   This sample uses  [product flavors](https://developer.android.com/studio/build/build-variants.html)  to replace modules at compile time, providing fake data for both manual and automated testing.
-   This version uses Rx to handle asynchronous.

This version of the app includes a number of unit tests which cover presenters, repositories. The sample also includes UI tests, that rely on fake data, and are facilitated by dependency injection to provide fake modules. For more information on using dependency injection to facilitate testing, see  [Leveraging product flavors in Android Studio for hermetic testing](https://android-developers.googleblog.com/2015/12/leveraging-product-flavors-in-android.html).
  

