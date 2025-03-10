# themirrazz' privacy policy
Last updated: 10 March 2025

## Introduction
Thanks for checking out my website! Like most other websites, mine uses things like browser cookies and collects information. This privacy policy tells you what information I collect, how I use your information, and who I share it with.

This privacy policy only applies to my main website. My other websites have their own privacy polices, unless it's explicitly stated or their privacy policy is missing.

## What types of data do you collect?
When you visit my website, your browser automatically sends some information to it. This information includes:
* The IP address of your device or router
* Your general location
* The type of browser or device you're using
* Any cookies that are stored on your device
* The URL of the page that you visit
* Any URL parameters (eg search query) present when the page load starts
* The time and date that the page load started

When an error occurs on the website, my custom sentry implementation collects data about the error and about your device. This information includes:
* The type of error that occured
* A message explaining the error in depth
* Information about the error's [stack](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error/stack), if available
* Information about the [cause](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error/cause) of the error, if available
* Which browser and which browser version you're using
* Which operating system and device you're using
* The time and date that the error occured

## How do you use it?
I use the information sent with each request to:
* Load the correct page and content
* Determine which country you are in for georestriction purposes
* Make my website work by sending pages back to you
* Help prevent people from abusing my website or, by extent, Vercel

I use the information collect from sentry data to:
* Fix bugs and glitches in my code
* Improve the browsing experience for all users
* Allow my website to run properly on a wider range of platforms
* Create, roll out, tweak, and improve experimental features

## How long do you keep data?
My website's hosted on Vercel, so I don't directly have access to the data sent with each request.

However, I usually just keep sentry data until the error is fixed. Sometimes, I might keep it longer, or even forever, but don't worry - sentry data doesn't have personal information. If you're using a custom user-agent that could expose personal information about you (eg `Chrome/130.94.25 MyName/FredKendricks)`) then I'll probably delete that part or the entire user agent.

## Do you use cookies?
"Cookies" are small pieces of data that websites can store on your computer. Whenever your browser makes a request to a website, the server can both read and change its own cookies. Cookies are sent in a header along with every request to a website. In addition, interactive code ("JavaScript") on a webpage can also read and set cookies.

When you change settings, like putting my website in Japanese, or turning on dark mode, my website stores that information in your browser. It use something called "local storage" to keep these settings. Local storage is another way to store data on your device. Unlike traditional cookies, local storage values aren't included in each request, and can only be accessed from JavaScript. My website does this to prevent your settings from getting shared to Vercel, or hackers (through a possible [man-in-the-middle](https://en.wikipedia.org/wiki/Man-in-the-middle_attack) attack).

However, local storage is only available in more modern versions of browsers. If you're using Internet Explorer 7 or older, local storage isn't available. My website use an IE-specific storage implementation for versions 5.5 through 7 to protect your privacy, which acts similar to localStorage. If you are using an older version of a browser that is not Internet Explorer, we will fallback to using traditional cookies, meaning that your settings will be sent to Vercel and any hackers (MITM).

## Do you track users?
No. I don't track users or have analytics. I only have a custom sentry implementation for collecting error logs, which attempts to remove sensitive information.

## How can I limit my data being collected?
My website responds to both Do Not Track (DNT) and Global Privacy Control (GPC). When you enable one of these, my sentry service will collect less information when an error occurs:
* The URL of the page you are on will be removed
* The timestamp will be rounded to each 10 second instead of each millisecond
* Information about your browser, OS, and device won't be sent

Please note that browser information is sent with each request, so Vercel might still collect information about your browser. (As mentioned above, we currently can't control this.)

I've also taken precautions to help protect your privacy even when DNT or GPC are disabled:
* My website doesn't send back your local IP address (eg local proxy for Windows 98)
* It doesn't send back URL parameters (eg search query) to prevent data leakage

## Do you sell or share users' data?
I don't sell users' information to third-parties, but I might share data with third-parties if I need to for a feature to work.

For example, if I added a mailing list/newsletter feature (which I'm not going to), your email address (and the fact you visited my website at one point) might get shared with MailChimp.

## Who do you share it with?
My website is hosted on Vercel. This means that Vercel receives information about all requests made, along with all of the header data. I cannot control or turn this off at the moment.

To learn about how Vercel handles your data, please read [their privacy policy](https://vercel.com/legal/privacy-policy).

In addition, when you click any third-party links (eg a YouTube link) on my website, you are agreeing to their terms of service and privacy policy. My privacy policy does not apply to linked third-party websites.

Some commonly linked websites are [YouTube](https://policies.google.com/privacy), [SoundCloud](https://soundcloud.com/pages/privacy), [DeviantArt](https://www.deviantart.com/about/policy/privacy), and [Archive Of Our Own](https://archiveofourown.org/privacy). To learn about how they handle your data, please read their privacy policies.

## Wait...  You can change this?!
Yes. If I start collecting more types of data, or add features that change how data is used, I'll edit this policy. You can (and should) check back regularly to see if there's any changes to how your data is being used.

All previous versions of privacy policies can be found on my GitHub at [themirrazz/privacy](https://github.com/themirrazz/privacy), starting with September 12, 2024 (the one before this privacy policy.)

By visiting this link, you agree to GitHub's privacy policy, which you can find [here](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
