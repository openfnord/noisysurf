# Noisysurf

Noisysurf is a plugin that creates meaningless web data by navigating your browser randomly around a list of news sites, to confound tracking & personalization algorithms and burst filter bubbles.
Here Noisysurf hopes to catch a lot of advertisement as this adds to traffic. So please disable adblockers when using Noisysurf to get the full traffic generated. BTW you can test your Adblocker with Noisysurf.

# Noisysurf is a modified fork of Noizy
Learn more about this project at [noiszy.com](https://noiszy.com/) and the [Noiszy blog](https://noiszy.com/blog/).

## Open source 
The original Noizy is open source under MIT Licence. Noizy was originally written by Angela Grammatas

https://github.com/openfnord/noiszy
https://github.com/noiszy/noiszy

I did the following modifications:
- Removed Google Analytics, as you do not want to be tracked, period.
- set the base timing to be very fast so more traffic is generated, while you can not read the news anymore. The original Noizy waited around (random) 1 Minute for a click or new page.
- Noisysurf is intended for traffic generation not for reading, so there is no setting to slow down surfing. Maybe in the future there will be a timing value in the menue for user-adjustment.
  As Noisysurf is needed just to generate as much "realistic" web traffic as possible, there is no need for such a surf timing setting at the moment.

## A note about tracking

I managed to remove Google Analytics, you do not want to be tracked, period.
The original noiszy contains google tracking.

## Timing
The timing can be adjusted in background.js: base_interval = 0.01 instead of 1. Use 1 or more for more human browsing and entertainment as you have about 1 minute left for reading. 
Use 0.01 for traffic generation. In the future there will be a parameter in the settings (options.html and options.js) to configure the base_interval of background.js which is used as factor for random number timing.

## Testing of a test version with firefox.
In the browser in about:config the setting "xpinstall.signatures.required" needs to be set to false to allow the installation of unsigned extensions (use with care!)
You can use the test_noisysurf.xpi which includes the newest modifications but is unsigned, or roll your own (just edit the java script and zip the content and rename the zip to xpi) noisysurf

# There is an official version of Noisysurf signed by mozilla.

https://raw.githubusercontent.com/openfnord/noisysurf/refs/heads/main/noisysurf_signed.xpi

https://addons.mozilla.org/en-US/firefox/addon/noisysurf/

Have fun with generated noisy webtraffic.
