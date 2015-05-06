#WDPR iOS Testing Frameworks

###Table of Contents

 0. [Preface](#preface)
 1. [Introduction](#introduction)
 2. [The Recommended Frameworks](#the-recommended-frameworks)
 3. [How to set up your test environment](#how-to-set-up-your-test-environment)

##Preface
This document describes the recommended frameworks for testing iOS applications. The recommended frameworks cover basic unit testing, performance testing, integration testing, and functional/UI testing.

If you are trying to choose a framework for testing your application or are trying to configure your test environment, the following is RA's recommendation for setting up the ideal testing environment.

For installing additional frameworks, RA recommends that you use [Cocoapods](https://cocoapods.org).

##Introduction
Mobile applications rely heavily on user experience as a cornerstone of their value, and as such, it is crucial that mobile applications provide exceptional user experience. To insure the best possible user performance, we find it helpful to create tests to insure quality in three key areas:

>	**Unit Tests:** Guarantee the stability of your application's logic in the smallest possible increments

>	**UI/Functional Tests:** Verify the reliability of your application's user interface and user interactions

>	**Performance Tests:** Test the speed of your application to insure a quick, responsive, delightful experience for the user

Each of these areas is critical to the construction of a great user experience, and each is subject to its own unique pitfalls.  Use of the following testing frameworks will help to guarantee the best user experience possible.

##The Recommended Frameworks

###XCTest
XCTest is the testing framework built directly into XCode (Xcode 5 and later) - XCTest provides a solid foundation for writing your tests, including support for asynchronous tests, performance tests, and no additional set up for any project created in XCode 5 or later.

###OCMockito
OCMockito is a framework that allows for the creation, verification, and stubbing of mock objects. This provides the capability to simulate objects for tests that otherwise may be difficult to test. 

###Calabash
Calabash is an automated testing technology that allows for the creation of Functional/UI tests that leverage the built in Accessibility library.

##What the decision was guided by (why these frameworks)
In determining which frameworks were best used to create a comprehensive and easy to use suite, a number of frameworks were considered, and judged on several different criteria.

###Unit Testing Tools
| Framework | Installation | Language/Reability | Asynchronous Testing | Performance Testing | Mock Objects | Compatibility with Jenkins |
| --------- | ------------ | ------------------ | -------------------- | ------------------- | ------------ | -------------------------- |
| XCTest | Built into XCode 5 and later, no additional setup required | Objective C, easily written and understood | Available | Available | N/A | Compatible |
| OCMock | Can be downloaded via Cocoapods, Github, or [OCMock.org](http://ocmock.org/download/), but requires additional steps to setup | Objective C | N/A | N/A | Available | Compatible |
| OCMockito | Installs easily with Cocoapods - also installs OCHamcrest | Uses OCHamcrest matcher library to simplify assertion statements, integrates well with Objective C | N/A | N/A | Available | Compatible |
| Kiwi | Installs with Cocoapods, operates alongside XCTest, not on top | Objective C, uses custom expectations | Available | N/A | Available | Compatible |
| Specta/Expecta | Installs easily with Cocoapods | Uses custom Expecta matchers - very easy to read | Available | N/A | N/A | Compatible |

###Functional/UI Testing Tools
| Framework | Installation | Language/Reability | Functional/UI Testing Capabilities | Compatibility with Jenkins | Notes |
| --------- | ------------ | ------------------ | ---------------------------------- | -------------------------- | ----- |
| Zucchini | Multi-step installation, requires homebrew, coffee-script, and keeps your tests in a seperate projects | Tests are written using Coffeescript, and uses screenshots to confirm test results | Capable of running UI tests on devices and simulator | Compatible, but doesn't support all features |
| Calabash | Provides in depth instructions for quick automatic setup, setup using cocoapods, and custom manual setup on github | Tests are written using Gherkin, and are easy to read. | Uses accessibility labels/ids to identify elements for testing, and supports testing on device and in simulator | Compatible | Available for both iOS and Android |
| KIF | Installs easily with Cocoapods | Tests are written in Objective C, are very verbose | Uses accessibility labels/ids to identify elements for testing, and supports testing on device and in simulator | Compatible | Does not provide simple support for screenshots while testing |

Having reviewed each of the above frameworks, XCTest, OCMockito, and Calabash were selected based on their ease of installation, the features they provide, and the readability of their tests.

##How to set up your test environment
0. **If your project was created using a version of XCode earlier than XCode 5** you may need to create a test target for your project to incorporate XCTest. To do this, see [Add Testing to Your App](https://developer.apple.com/library/ios/documentation/DeveloperTools/Conceptual/testing_with_xcode/testing_1_quick_start/testing_1_quick_start.html#//apple_ref/doc/uid/TP40014132-CH2-SW3) in the Apple Developer Library
1. Make sure you have Cocoapods set up on your machine, instructions on how to set up Cocoapods are available at [Cocoapods.org](https://guides.cocoapods.org/using/getting-started.html#getting-started)
2. Make sure that your project is configured to use Cocoapods, instructions are available at [Cocoapods.org](https://guides.cocoapods.org/using/using-cocoapods.html)
3. Follow [these instructions](https://github.com/jonreid/OCMockito#how-do-i-add-ocmockito-to-my-project) to add OCMockito to your project
4. Follow [these instructions](https://github.com/calabash/calabash-ios#setup-and-requirements) to setup Calabash 
