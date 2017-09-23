# Simplicity
A theme made for simplicity and ease of use

Feel free to use it, leave feedback and suggest new features!
For the best results, **use the dark theme**.

Designed by *THEE Yandere-Chan* ; latest version: **3.1.0**.

# Dynamic Import
Paste this link in your Custom CSS section if you want to
dynamically load the theme without having to download any files. Besides the main theme
```css
/* IMPORT CSS FROM GITHUB */

/* Mod Loader */
@import url("https://cdn.rawgit.com/THEEYandereChan/Simplicity/master/mods/UserPopoutsUpgraded.theme.css");

/* Load Base theme */
@import url("https://cdn.rawgit.com/THEEYandereChan/Simplicity/master/themes/Simplicity%20Beta.theme.css");
/* ===== CUSTOMIZABLE COLORS ===== */

:root {
	--main-color: #808080;
	--hover-color: #6f182a;
	--bgurl : url(https://raw.githubusercontent.com/THEEYandereChan/Simplicity/master/backgrounds/wallhaven-436907.jpg);
}
```

# Dedicated Import
Paste this in your theme.css file if you want to always import when you start discord
Use this to download the files
```css
//META{"name":"Simplicity Auto","description":"A simplistic theme compatible with BD and Stylish","author":"THEE Yandere - Chan","version":"3.1p"}*//{}

	/* IMPORT CSS FROM GITHUB */
	@import url("https://cdn.rawgit.com/THEEYandereChan/Simplicity/master/themes/Simplicity%20Beta.theme.css");


/*
===== IMPORTANT =====
CHANGE DISCORDS THEME TO DARK THEME IN APPEARANCE SETTINGS FOR THIS THEME TO WORK!
===== CUSTOMIZABLE COLORS =====
*/

:root {
	--main-color: #93261a;
	--hover-color: ##6F182A;
	--popoutColor: #000000;
	 --bgurl: url(https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-99007.jpg);
	--backdrop: url(https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-509261.jpg);
	--chat-text-color: #E3D4E7;
 }


/* Mod Loader */

/** PikaDude's Fade Animations **/
@import "https://rawgit.com/PikaDude/Discord-Fade-Anims/master/Discord-Fade-Anims.css";
/** TriggerRimfire's Avatar Shadow **/
@import "https://rawgit.com/TriggerRimfire/48b3303f4032fffd952c108260a059a4/raw/302f0672b2b7246a26dc2af0fa43bce90955e68b/discord-avatar-shadow.css";
/** jakeoid's Emoji Animations **/
@import "https://rawgit.com/jakeoid/discord-emoji-anim/master/stylesheet.css";
/** Vap0r1ze's Nitro Badges **/
@import "https://rawgit.com/Vap0r1ze/Discord-Nitro-Badges/master/nitro.css";

/** end **/

/** Ovyerus' Edited Pencil **/

.message-group .comment .edited {
    font-size: 0;
    width: 13px !important;
    height: 13px !important;
    display: inline-block;
    background-image: url(https://cdn.rawgit.com/twitter/twemoji/gh-pages/svg/270f.svg);
    background-size: 100%;
    opacity: 0.5;
    line-height: 23px;
    transition: opacity 0.2s;
}

.message-group .comment .edited:hover {
    opacity: 1;
}

/** Lewis' Mods (should get around to labelling these) **/

.app {
   background: rgba(0, 0, 0, 0.75);
}



.friends-icon {
   background-image: url(https://storage.googleapis.com/material-icons/external-assets/v4/icons/svg/ic_question_answer_white_24px.svg) !important;
   opacity: 0.8;
   margin-top: 4px;
   background-size: 50%!important;
}

.user-popout .body {
   background: rgb(0, 46, 46);
}

.user-popout .footer {
   background: rgb(0, 35, 35);
   border-top: 0px;
}

.note textarea:focus {
   background: #332e2e;
}

/** Slider white bar fix **/

.scroller {
	overflow-x: hidden !important;
}




@import url("https://cdn.rawgit.com/THEEYandereChan/Simplicity/master/mods/UserPopoutsUpgraded.theme.css");

/* Sublime Text Highlighting */


.css .hljs-tag,
.css .hljs-important,
.css .hljs-at_rule,
.css .hljs-keyword {
	color: #f92672 !important;
}
.css .hljs-class,
.css .hljs-id {
	color: #a6e300 !important;
}
.css .hljs-value,
.css .hljs-hexcolor,
.css .hljs-number,
.css .hljs-function {
	color: rgba(255, 255, 255, 0.8) !important;
}
.css .hljs-attribute {
	color: #82d4e5 !important;
}
.css .hljs-comment {
	color: #686545 !important;
}
.css .hljs-pseudo {
	color: #fff !important;
}

/* ===== CUSTOMIZABLE COLORS ===== */
/*
:root {
	--main-color: #93261a; /* Pink */ /*
	--hover-color: #8c2216; /* Violet/Dark Purple */
	/*--popoutColor: #000000;
	 --bgurl: url(https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-226153.jpg);
	--backdrop: url(https://wallpapers.wallhaven.cc/wallpapers/full/wallhaven-509261.jpg);
	--chat-text-color: #E3D4E7;
}
*/

/* Do not delete this it regulates the background Image! */
body {
  background: var(--bgurl) !important;
  background-size: cover !important;
  background-attachment: fixed !important;
  background-position: center !important;
  background-repeat: no-repeat !important;
}
/* User popout */

.userPopout-4pfA0d {
	background: var(--popoutColor);
}

.userPopout-4pfA0d .body-3rkFrF, .headerNormal-1cioxU, .footer-2J5zqP,.quick-message {
  background: transparent !important;
  background-color: transparent !important;
}
[class*=userPopout] [class*=avatarWrapperNormal] [style*=image] {background-color:unset;width:100%;height:242px;width:242px;background-size:contain;background-position:center;background-repeat:no-repeat;border-radius:0;border:none;}
[class*=userPopout] [class*=avatarWrapperNormal] {margin:4px 4px 0;position:absolute;top:0;left:0;}
[class*=userPopout] [class*=header]:hover [class*=avatarWrapperNormal] {-webkit-filter: grayscale(14%);transition: -webkit-filter 500ms ease-out;}
[class*=userPopout] [class*=headerNormal],[class*=userPopout] [class*=headerStreaming]{height:254px;transition: -webkit-filter 100ms;background:#fff;padding:0}
[class*=userPopout] [class*=headerText] {height:236px;width:200px;overflow:hidden;position:absolute;top:2px;display:flex;flex-flow:column;pointer-events:none;justify-content:flex-end}
[class*=userPopout] [class*=avatarWrapperNormal] [class*=avatarHint-] {background: linear-gradient(to bottom, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0) 80%, rgba(0,0,0,0) 100%);margin:0;box-shadow:none;opacity:0;border-radius:0;transition: opacity 180ms ease-out 100ms;}
[class*=userPopout] [class*=avatarWrapperNormal]:hover [class*=avatarHint-] {background: linear-gradient(to bottom, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0) 80%, rgba(0,0,0,0) 100%);transition:opacity 300ms ease-in 80ms;opacity:1;}
[class*=userPopout] [class*=headerText] div[class*=header] {background: linear-gradient(to right, rgba(0,0,0,0) 0%,rgba(0,0,0,0.4) 15%,85%,rgba(0,0,0,0) 100%);width: 200px;max-width: 200px;padding:0;order:2;opacity:1;transition: opacity 200ms ease-in;transition-delay: 170ms;min-height:19px;pointer-events:auto}
[class*=userPopout] .username-wrapper .nickname {margin-bottom:4px;}
[class*=userPopout] [class*=headerText] [class*=ctivity] {height:auto;max-height:40px;overflow:hidden;}
[class*=userPopout] [style*=image] [class*=tatus] {bottom:-8px;width:100%;height:8px;left:0;box-shadow: inset 0 0 0 1.8px rgba(255,255,255,.2);border-radius:0;pointer-events:none;}
[class*=userPopout] [class*=header]:hover [class*=avatarWrapperNormal] [class*=tatus]{-webkit-filter: contrast(105%);transition: -webkit-filter 480ms ease-out;}
[class*=userPopout] [class*=header] [class*=headerText] [class*=ctivity],.user-popout .header:not(:hover) .creation-date-wrapper {opacity: 0;transition: opacity 200ms,margin-bottom 270ms ease-out;}
[class*=userPopout] .header .creation-date-wrapper {padding:3px 0;margin-bottom:145px;order:1;transition:margin-bottom 170ms ease-in-out;min-height:unset;}
[class*=userPopout] .header:hover .creation-date-wrapper, [class*=header]:not(:hover) [class*=headerText] [class*=ctivity]{margin-bottom:-28px;}
[class*=userPopout] [class*=header]:hover [class*=headerText] [class*=ctivity]{margin-bottom:4px;opacity:1}
[class*=userPopout] [class*=header]:hover [class*=headerText] div[class*=ctivity]:empty{margin-bottom:-28px;}
[class*=userPopout] [class*=headerStreaming] [style*=image] [class*=tatus] {border:none;}
[class*=userPopout] a[class*=Live] {position:fixed;left:0;right:0;top:20px;z-index:2;border:none!important;border-bottom:1px solid rgba(255,255,255,.08);padding:3px 25px;pointer-events:auto;width:200px;height:16px;}
[class*=userPopout] a[class*=Live]:hover {background:transparent;}
[class*=userPopout] a[class*=Live] [class*=con] {position:absolute;z-index:-1;width:200px;height:100%;border-radius:0;background:linear-gradient(to right,transparent,#f04747 15%,#f04747 85%,transparent);animation:l-p 1s ease-in-out infinite alternate}
@keyframes l-p {0%,20%{opacity:.6} 0%,10%,30% {opacity:1}}
[class*=userPopout] .member-roles {max-height: 90px;overflow-y: scroll;}
[class*=userPopout] .member-roles::-webkit-scrollbar {width:0;}
/* End user Popout Upgrade */

```

# Preview
![Preview](https://vgy.me/5UweEN.png)
