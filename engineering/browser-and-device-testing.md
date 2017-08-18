# Browser and device testing

_Our approach to testing on different platforms_

To make sure the final result works on as many platforms and devices as possible, we usually start testing early on. It’s important to emphasise that we can’t guarantee to cover all devices in the world, due to the vast amount of platforms and device resolutions, and the massive fragmentation in the Android market (10,000+ devices).

However we do have access to plenty of real devices that cover the most common screen resolutions on desktop, tablet and mobile as well as all popular operating systems (Windows, MacOS, Android and iOS).

As for the notoriously difficult Internet Explorer, we can cover version 9 upwards (which is already quite outdated), and usually use Microsoft’s very own [virtual machines](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/) to thoroughly test the user experience in their browsers.

Additionally, we use tools like [BrowserStack](https://www.browserstack.com/) to back up our results, which gives us access to a huge number of testing devices and browsers (including older versions of self-updating browsers like Chrome or Firefox).

We take testing seriously, and have years of experience with oddly behaving rendering engines and spending night shifts debugging weird Internet Explorer 7 bugs. While a project might not always have the budget to test as thoroughly as we might like, we’re aware of the risks that come with inadequate testing. We approach browser and device testing with accessibility and usability in mind, to provide the best possible experience for the user groups we’re targeting.
