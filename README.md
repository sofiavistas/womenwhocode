# womenwhocode

My learning resources used on the process of setting up a mobile automation framework for our Android app. My starting point:
few Java, no Espresso and vague Jenkins knowledge

## Java

Brush up some before diving in Espresso: https://www.codecademy.com/learn/learn-java

## Espresso

Step 1 –  Start here:

```
http://www.vogella.com/tutorials/AndroidTestingEspresso/article.html
```

Step 2 – Grab a cheat sheet:

```
https://google.github.io/android-testing-support-library/docs/espresso/cheatsheet/
```
Step 3 – Start playing with Espresso Record feature:

```
https://developer.android.com/studio/test/espresso-test-recorder.html
```

Step 4 – Brew some coffee and read some Espresso examples:

```
https://github.com/googlesamples/android-testing/
```

 Step 5 – Grab some robots here:

```
https://realm.io/news/kau-jake-wharton-testing-robots/
```

## Jenkins

Our CI of choice. We use Jenkins Pipeline to have a "stage view" of each step. This is great to debug what whent wrong when building your pull requests.

```
https://github.com/jenkinsci/pipeline-plugin/blob/master/TUTORIAL.md
```

Your Android project can have a file called Jenkinsfile with the intended configuration. More flexible than using the UI offered by Jenkins.

```
https://jenkins.io/doc/book/pipeline/jenkinsfile/
```

## Spoon

Great report tool from folks at Square:

```
http://square.github.io/spoon/
```

## Android

How to go and mockup that API:
```
http://blog.davidmedenjak.com/android/2016/11/22/mocking-api-calls.html
```

### And then get some more

* [Advanced Android Espresso](https://www.youtube.com/watch?v=JlHJFZvZyxw) - by Chiu-ki Chan
* [UI Testing with Espresso](https://maven.apache.org/) - by Android Testing patterns series
* [Your Tests Aren't Flaky](https://www.youtube.com/watch?v=hmk1h40shaE) - by Google Tech Talks 2015

# FAQ

* I am having trouble when Espresso needs to wait for asyncronous tasks. What should I do?

Give your Espresso some Idle Resources. Great starting post here: http://matgom.com/tutorial/2016/02/21/IdlingResource.html

* I want to assert a more complicated View and I cannot get my way around in how to capture it. Are there other Matchers than the ones on the cheat sheet?

Yes, you can find several after a quick search. keywords: custom matcher your-fancy-element-name .
While you are here, probably you can implement your own custom matcher: http://qathread.blogspot.de/2014/03/descovering-espresso-for-android.html
