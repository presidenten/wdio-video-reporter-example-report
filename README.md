Example Allure report
=====================

This repo contains an example Allure report generated from three test-cases in the `wdio-video-reporter` demo with Webdriver.io v5.

Options used for the reporter:
```
  reporters: [
    [video, {
      saveAllVideos: true,        // If true, also saves videos for successful test cases
      videoSlowdownMultiplier: 3, // Higher to get slower videos, lower for faster videos [Value 1-100]
      videoRenderTimeout: 5,      // Max seconds to wait for a video to finish rendering
    }],
    ['allure', {
      outputDir: './_results_/allure-raw',
      disableWebdriverStepsReporting: true,
      disableWebdriverScreenshotsReporting: true,
    }],
  ],
```

All devices has their appium configurations extended with a custom `deviceType`-property set to: `phone`, `tablet` depending on device type.


For more information, see README at [https://github.com/presidenten/wdio-video-reporter](https://github.com/presidenten/wdio-video-reporter#wdio-video-reporter--)

