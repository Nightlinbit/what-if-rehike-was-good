# Configuration
*(Note: This document and its assets should be removed when Rehike has a configuration GUI.)*

*(Note 2: This document will only detail the configuration of `exp-signin-rework`, as that is the main branch being worked on currently)*

Rehike has a `config.json` file located in the root directory of it, next to `index.php` and such. This document will detail what each configuration key in it does.

## What the `config.json` file looks like

<pre>
{
    "useRingoBranding": true,
    "uploadMenuType": "MENU",
    "dateOnWatchSidebarItems": false,
    "useWebV2HomeEndpoint": false,
    "versionInFooter": true,
    "useReturnYouTubeDislike": true,
    "enableRehikeDebugger": false,
    "largeSearchThumbs": true,
    "byTextOnByline": false,
    "noViewsText": false,
    "movingThumbnails": true,
    "guideOnWatchPage": false,
    "hhCSSFixes": true
}
</pre>

|Contents                                                 |
|---------------------------------------------------------|
| 1. [`useRingoBranding`](#useringobranding)              |
| 2. [`uploadMenuType`](#uploadmenutype)                  |
| 3. [`dateOnWatchSidebarItems`](#dateonwatchsidebaritems)|
| 4. [`useWebV2HomeEndpoint`](#usewebv2homeendpoint)      |
| 5. [`versionInFooter`](#versioninfooter)                |
| 6. [`useReturnYouTubeDislike`](#usereturnyoutubedislike)|
| 7. [`enableRehikeDebugger`](#enablerehikedebugger)      |
| 8. [`largeSearchThumbs`](#largesearchthumbs)            |
| 9. [`byTextOnByline`](#bytextonbyline)                  |
| 10. [`noViewsText`](#noviewstext)                       |
| 11. [`movingThumbnails`](#movingthumbnails)             |
| 12. [`guideOnWatchPage`](#guideonwatchpages)            |
| 13. [`HHCSSFixes`](#hhcssfixes)                         |


## `useRingoBranding`

Enables/disables the use of the current logo, and a bright red color.

`true`:

![The top left of the YouTube homepage, with the current logo and bright red.](assets/config/useRingoBranding-true.png)

`false`:

![The top left of the YouTube homepage, with the old logo from 2015/2016, and a darker red color.](assets/config/useRingoBranding-false.png)

## `uploadMenuType`

Sets the display of the "Upload" menu/button found in the top right of the page.

`"BUTTON"`:

![The top right of the YouTube masthead, with a default-styled button that reads "Upload".](assets/config/uploadMenuType-BUTTON.png)

`"ICON"`:

![The top right of the YouTube masthead, with an icon-button, depicting an arrow facing up, with a horizontal line below it.](assets/config/uploadMenuType-ICON.png)

`"MENU"`:

*(Note: You can use any value that is not "BUTTON" or "ICON" for this, as it is the default and the fallback.)*

![The top right of the YouTube masthead, with a icon-button, depicting a camera with a plus icon inside it. Below it is a menu with the options "Upload video" and "Go live".](assets/config/uploadMenuType-MENU.png)

## `dateOnWatchSidebarItems`

Enables/disables showing relative date on the watch page's "Up next" section.

`true`:

![A recommended video on the watch page, with the meta line reading "36,773,232 views • 1 year ago"](assets/config/dateOnWatchSidebarItems-true.png)

`false`:

![A recommended video on the watch page, with the meta line reading "36,773,232 views". Note the lack of "1 year ago".](assets/config/dateOnWatchSidebarItems-false.png)

## `useWebV2HomeEndpoint`:

Enables/disables the homepage which uses the WEB V2 endpoint. This homepage has no shelves. Instead it is all one section. However, you gain the ability to view the videos in a list view.

`true`:

|Grid|List|
|----|----|
|![The shelfless WEB V2 homepage in a grid format](assets/config/useWebV2HomeEndpoint-true-grid.png)|![The shelfless WEB V2 homepage in a list format](assets/config/useWebV2HomeEndpoint-true-list.png)|

`false`:

![The shelved ANDROID homepage in Hitchhiker's format.](assets/config/useWebV2HomeEndpoint-false.png)

## `versionInFooter`

Shows the Rehike version in the footer, which links to the version page.

`true`:

![The footer with the Rehike version in the primary links.](assets/config/versionInFooter-true.png)

`false`:

![The footer without the Rehike version in the primary links.](assets/config/versionInFooter-false.png)

## `useReturnYouTubeDislike`

Enables/disables showing dislikes and sparkbar on watch page, using data from the [Return YouTube Dislike](https://returnyoutubedislike.com/) API.

`true`:

![The bottom right of the main watch panel, with dislikes and the sparkbar.](assets/config/useReturnYouTubeDislike-true.png)

`false`:

![The bottom right of the main watch panel, without dislikes and the sparkbar.](assets/config/useReturnYouTubeDislike-false.png)

## `enableRehikeDebugger`

Enables the Rehike debugger. Also useful if errors somehow get spat out into the document and fuck up your entire experience.

## `largeSearchThumbs`

Enables/disables large thumbnails on search.

`true`:

![A video on search, with a large thumbnail and title text.](assets/config/largeSearchThumbs-true.png)

`false`:

![A video on search, with the regular tile video size.](assets/config/largeSearchThumbs-false.png)

## `byTextOnByline`

Enables/disables the showing of "by" before the author's name on videos.

`true`:

![A video, with the byline reading "by Rick Astley".](assets/config/byTextOnByline-true.png)

`false`:

![A video, with the byline reading "Rick Astley".](assets/config/byTextOnByline-false.png)

## `noViewsText`

Enables/disables the hiding of the "views" text after the view count on the watch page.

`true`:

![The bottom right of the main watch panel, with the view count reading "1,248,508,383".](assets/config/noViewsText-true.png)

`false`:

![The bottom right of the main watch panel, with the view count reading "1,248,508,383 views".](assets/config/noViewsText-false.png)

## `movingThumbnails`

Enables/disables animated previews upon hovering over a video.

`true`:

![A homepage video being hovered over, showing an animated preview of the video.](assets/config/movingThumbnails-true.png)

`false`:

![A homepage video being hovered over, with no preview, and instead continuing to show the thumbnail.](assets/config/movingThumbnails-false.png)

## `guideOnWatchPage`

Enables/disables guide pinning on the watch page.

`true`:

![Watch page, with the guide pinned to the left side of the screen, like many other pages.](assets/config/guideOnWatchPage-true.png)

`false`:

![Watch page without any guide, like normal.](assets/config/guideOnWatchPage-false.png)

## `hhCSSFixes`

Consistency/bug fixes for default Hitchhiker CSS. This may conflict with CSS themes, so set it to `false` if you encounter any issues with themes.
