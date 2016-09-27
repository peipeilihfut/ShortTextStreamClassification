# ShortTextStreamClassification
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
<!-- saved from url=(0042)http://adapt.seiee.sjtu.edu.cn/similarity/ -->
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd"><HTML><!-- v:10.0.7.13 --><HEAD 
id="ctl00_ctl00_HeadTag"><META content="IE=9.0000" http-equiv="X-UA-Compatible">

<META http-equiv="X-UA-Compatible" content="IE=9">
<META http-equiv="Content-Type" content="text/html; charset=gb2312">
<META name="assetType" content="Web Page"><TITLE>Concept based Short Text Stream Classification with Topic Drifting Detection
				 </TITLE><LINK title="Microsoft Research - Downloads" href="http://research.microsoft.com/rss/downloads.xml" 
rel="alternate" type="application/rss+xml"><LINK title="Microsoft Research - Kinect for Windows SDK" 
href="http://research.microsoft.com/en-us/um/redmond/projects/kinectsdk/kdkrss.xml" 
rel="alternate" type="application/rss+xml"><LINK title="Microsoft Research - News" 
href="http://research.microsoft.com/rss/news.xml" rel="alternate" type="application/rss+xml"><LINK 
title="Microsoft Research - Publications" href="http://research.microsoft.com/rss/publications.xml" 
rel="alternate" type="application/rss+xml"><LINK title="Microsoft Research - Research Lectures" 
href="http://research.microsoft.com/rss/researchLectures.xml" rel="alternate" 
type="application/rss+xml"><LINK title="Microsoft Research - Visiting Speaker Lectures" 
href="http://research.microsoft.com/rss/visitingSpeakers.xml" rel="alternate" 
type="application/rss+xml">     
<STYLE type="text/css">
      

/* fonts and font formatting*/
.b, .people .GroupContact, .people .person .lastname, #contentArea #dedlM table.inner td.left, .pubD #contentArea td.heading {font-weight:bold;}
.n, #chTB #chTer .item, #contentArea font.ImageBlock, span.ImageBlock, .versal #zone1 div.infographic h5, #contentArea h1, #contentArea .H1, #contentArea h2, #contentArea .H2, #contentArea h3, #contentArea .H3, #contentArea h4, #contentArea .H4, #contentArea h5, #contentArea .H5, #contentArea h6, #contentArea .H6, #contentArea .title, #contentArea .dirTagLink, #contentArea .byLine, #contentArea .copyright, #contentArea .relatedLinksHead, #contentArea .smallText, #contentArea .largeText, #contentArea #dedlM table.inner td, #contentArea .rssM .date, .pubD #contentArea td {font-weight:normal;}


.f1, #contentArea h6, #contentArea .H6 {font-family:'Courier New';}
.f2, #contentArea h1, #contentArea .H1, #contentArea h2, #contentArea .H2, #contentArea h3, #contentArea .H3, #contentArea h4, #contentArea .H4, #contentArea .title {font-family:Georgia;}
.f3, body, #chTB #chSearch input[type="text"], #chTB #chSearch #cst, #chNav #chPM, #contentArea #dedlM button, #contentArea font.ImageBlock, span.ImageBlock, #contentArea h5, #contentArea .H5, .versal #zone1 div.infographic h5, #chTB #chSearch div, #contentArea .dirTagLink, #contentArea .byLine, #contentArea .copyright, #contentArea .relatedLinksHead, #contentArea .smallText, #contentArea .largeText, #contentArea #dedlM table.inner td, #contentArea .rssM .date, .lNavVertical ul, .lNavVerticalTabs ul, .pubD #contentArea td, .pubD #contentArea td.heading {font-family:Verdana;}
.fs1, #contentArea H1 .ImageBlock, #contentArea .H1 .ImageBlock {font-size:46%!important;}
.fs2, #contentArea H2 .ImageBlock, #contentArea .H2 .ImageBlock {font-size:53.333%!important;}
.fs3, #footer {font-size:60%;}
.fs4, #contentArea H3 .ImageBlock, #contentArea .H3 .ImageBlock {font-size:66%!important;}
.fs5, .versal .date, #crumbBar, .pop ul li {font-size:70%;}
.fs6, #contentArea H4 .ImageBlock, #contentArea .H4 .ImageBlock {font-size:73%!important;}
.fs7, #contentArea, .pop .h, #contentArea font.ImageBlock, span.ImageBlock {font-size:80%;}
.fs8 {font-size:24px;}
.fs9, .versal #zone1 div.infographic, #contentArea #dedlM table.outer td.right, #contentArea #dedlM table.inner td {font-size:85%;}
.fs10, #contentArea .dirTagLink, #contentArea .byLine, #contentArea .copyright, #contentArea .rssM .date {font-size:87%;}
.fs11, #contentArea .smallText {font-size:88%;}
.fs12, #contentArea .relatedLinksHead {font-size:95%;}
.fs13, body, .versal #zone1 div.infographicInner, #contentArea .conM ul ol, #contentArea .conM ul ul ul ul, #contentArea .conM ul ul, #contentArea .conM table, #contentArea .conM ol ol, #contentArea .conM ul ol, #contentArea .conM ol ol ol, #contentArea .conM ol ol ol ol, #contentArea .conM ul ul ul, #contentArea .conM ul ul ul ul, #contentArea .conM ul ul, #contentArea .conM li p, #contentArea .conM table, #contentArea .peM  .item, #contentArea .peMi .item, .pubD #contentArea td, .pubD #contentArea td.heading {font-size:100%;}
.fs14, #contentArea H6 .ImageBlock, #contentArea .H6 .ImageBlock {font-size:100%!important;}
.fs15, #contentArea h4, #contentArea .H4, #contentArea h6, #contentArea .H6 {font-size:109%;}
.fs16, .versal #zone1 div.infographic h5 {font-size:110%;}
.fs17 {font-size:120%;}
.fs18, #contentArea h3, #contentArea .H3 {font-size:121%;}
.fs19, #contentArea .largeText {font-size:125%;}
.fs20, #contentArea h2, #contentArea .H2 {font-size:150%;}
.fs21, #contentArea h1, #contentArea .H1 {font-size:175%;}
.fs22, #contentArea .title {font-size:225%;}
.fs23, #chTB #chTer .item {font-size:11px;}
.fs24, #chNav #chS li, #chNav #chPM {font-size:12px;}
.fs25, #chTB #chSearch input[type="text"], #chTB #chSearch #cst, #chTB #chSearch div {font-size:13px;}
.fs26, #chNav #chP td div {font-size:14px;}
.fs27, #chNav #chP td.sel a, #contentArea h5, #contentArea .H5  {font-size:15px;}
.fs28, #contentArea #dedlM button {font-size:16px;}
.fsi, #chTB #chSearch input[type="text"], #chTB #chSearch #cst, #contentArea h4, #contentArea .H4 {font-style:italic;}
.fsn, #chTB #chSearch #cst.sel, #contentArea font.ImageBlock, span.ImageBlock {font-style:normal;}

.tdn, .versal #versalBtm a:hover, #chTB a, #chNav #chP a, #chNav #chS a, #chNav #chPM a, #crumbBar a, #contentArea a, #footer a {text-decoration:none;}
.tdni, .lNavVertical a, .lNavHorizontal a,.lNavVertical a:hover, .lNavHorizontal a:hover,.lNavVertical a:visited, .lNavHorizontal a:visited, .lNavVerticalTabs a, .lNavHorizontalTabs a,.lNavVerticalTabs a:hover, .lNavHorizontalTabs a:hover,.lNavVerticalTabs a:visited, .lNavHorizontalTabs a:visited {text-decoration:none!important;}
.tdu, #chNav #chPM a:hover, #crumbBar a:hover, #contentArea a:hover {text-decoration:underline;}

.tt1, #contentArea .relatedLinksHead {text-transform:uppercase;}

.to1, #bcHolder {text-overflow:ellipsis;}

.crP, #chTB #chSearch #goButton, #crumbBar a, #chTB #chTer .item, #crumbBar #tools img, #contentArea #dedlM button {cursor:pointer;}

/*height and width */
.mh1, .compositeModule_2Zone > div.zone, .compositeModule_3Zone > div.zone, .compositeModule_4Zone > div.zone, .compositeModule_4Zone > div.zone, .compositeModule_1_2Zone > div.zone:first-child, .compositeModule_1_2Zone > div.zone + div.zone, .compositeModule_2_1Zone > div.zone:first-child, .compositeModule_2_1Zone > div.zone + div.zone, .compositeModule_1_3Zone > div.zone:first-child, .compositeModule_1_3Zone > div.zone + div.zone, .compositeModule_3_1Zone > div.zone:first-child, .compositeModule_3_1Zone > div.zone + div.zone, .compositeModule_1Zone > div.zone, .compositeModule_1_2_1Zone > div.zone:first-child, .compositeModule_1_2_1Zone > div.zone + div.zone + div.zone, .compositeModule_1_2_1Zone > div.zone + div.zone {min-height:10px;}

.ht1, .compositeModule_2Zone, .compositeModule_3Zone, .compositeModule_4Zone, .compositeModule_1_2Zone, .compositeModule_2_1Zone, .compositeModule_1_3Zone, .compositeModule_3_1Zone, .compositeModule_1Zone, .compositeModule_1_2_1Zone {height:100%;}
.ht0, .cl {height:0;}
.ht2, .cr, hr {height:1px;}
.ht3, #bGrad {height:10px;}
.ht4, #chTB #chSearch div, #chTB #chSearch input[type="text"], #chTB #chSearch #cst {height:18px;}
.ht5, #chNav #chS {height:24px;}
.ht6, #contentArea #dedlM div.btm, #footer {height:25px;}
.ht7, #shadow #top {height:26px;}
.ht8, #chNav #chP {height:30px;}
.ht9, #contentArea #dedlM button {height:37px;}
.ht10, #chTB #chLogo img {height:41px;}
.ht11, #chTB #chSearch {height:48px;}
.ht12, #chNav #chPM {height:53px;}
.ht13, #chTB {height:60px;}
.ht14, #chNav {height:61px;}
.ht15, #contentArea #dpeM img, #contentArea .peMi img, #contentArea .videoM .SmallImageBlock, #contentArea .videoM .SmallImageBlock img {height:72px;}
.ht16, .people .person .BlankPictureDiv {height:75px;}
.ht17, #contentArea .peMi .itemShort {height:110px;}
.ht18, #contentArea .peMi .item {height:134px;}
.ht19, #contentArea .videoM .tile, #contentArea .videoM .tileExtra, #contentArea .videoM .tile > img, #contentArea .videoM .tileExtra > img, #contentArea .videoM .ImageBlock, #contentArea .videoM .ImageBlock img {height:150px;}
.ht20, #contentArea .videoM .tileExtra {height:185px;}

.w1, .compositeModule_1_2_1Zone > div.zone:first-child, .compositeModule_1_2_1Zone > div.zone + div.zone + div.zone {width:16%;}
.w2, #chTB #chTer .item {width:20%;}
.w3, .compositeModule_4Zone > div.zone {width:24%;}
.w4, .compositeModule_1_3Zone > div.zone:first-child, .compositeModule_3_1Zone > div.zone + div.zone {width:25%;}
.w5, .compositeModule_3Zone > div.zone, .compositeModule_1_2Zone > div.zone:first-child {width:32%;}
.w6, .compositeModule_2_1Zone > div.zone + div.zone, .fw .compositeModule_3Zone > div.zone, .fw .compositeModule_3Zone > div.zone + div.zone + div.zone, .fw .compositeModule_1_2Zone > div.zone:first-child {width:33%;}
.w7, .fw .compositeModule_3Zone > div.zone + div.zone {width:34%;}
.w8, #contentArea #dedlM table.inner td.left {width:40%;}
.w9, .compositeModule_2Zone > div.zone {width:49%;}
.w10, #contentArea #dedlM table.inner td.right {width:60%;}
.w11, .compositeModule_1_2Zone > div.zone + div.zone, .compositeModule_2_1Zone > div.zone:first-child, .compositeModule_1_2_1Zone > div.zone + div.zone {width:66%;}
.w12, .fw .compositeModule_1_2Zone > div.zone + div.zone, .fw .compositeModule_2_1Zone > div.zone:first-child {width:67%;}
.w13, .compositeModule_1_3Zone > div.zone + div.zone, .compositeModule_3_1Zone > div.zone:first-child {width:70%;}
.w14, .fw .compositeModule_1_3Zone > div.zone + div.zone {width:74.9%;}
.w15, .compositeModule_1Zone > div.zone, #chNav #chP table, #contentArea #dedlM table, #contentArea #dedlM table.inner {width:100%;}
.w16, #contentArea #dpeM img, #contentArea .peMi img {width:72px;}
.w17, .people .person, .people .person .BlankPictureDiv {width:75px;}
.w18, #contentArea .videoM .SmallImageBlock, #contentArea .videoM .SmallImageBlock img {width:96px;}
.w19, #contentArea .peMi .item, #contentArea .peMi .itemShort {width:134px;}
.w20, #chTB #chLogo img {width:143px;}
.w21, #cShare {width:150px;}
.w22, #contentArea #dedlM button {width:163px;}
.w23, #contentArea #dedlM table.outer td.right {width:164px;}
.w24, #contentArea .videoM .tile, #contentArea .videoM .tileExtra, #contentArea .videoM .tile > img, #contentArea .videoM .tileExtra > img, #contentArea .videoM .ImageBlock, #contentArea .videoM .ImageBlock img {width:200px;}
.w25, .versal #zone1 div.infographic {width:220px;}
.w26, .versal #zone2.conM {width:250px;}
.w27, .project1 #zone1 {width:280px;}
.w28, #chTB #chSearch #cst {width:295px;}
.w29, #contentArea #dedlM table.outer td.left {width:297px;}
.w30, #chTB #chSearch {width:316px;}
.w31, #chTB #chSearch input[type="text"] {width:323px;}
.w32, #chNav #chPM {width:324px;}
.w33, #chTer {width:360px;}
.w34, .project1 #zone2, .project1 #zone3, .versal #zone1.conM {width:560px;}
.w35, #chNav #chS {width:648px;}
.w36, #chNav #chP {width:649px;}
.w37, #bcHolder {width:810px;}
.w38, #chNav {width:978px;}
.w {width:994px;}
.sw {width:1002px;}

/* alignments */
.tac, .JustifyCenter, .people .person, #chTB #chTer .item {text-align:center;}
.taj, .JustifyFull {text-align:justify;}
.tal, .JustifyLeft {text-align:left;}
.tar, .JustifyRight, #contentArea #dedlM table.inner td.right {text-align:right;}
.vam, .versal #versalBtm img, #crumbBar #tools img, #contentArea #dedlM button img {vertical-align:middle;}
.vat, #contentArea #dedlM table.outer td, #crumbBar>a>img[alt="Home"] {vertical-align:top;}



/* colors */
.c1, .versal #zone1 div.infographic h5, #contentArea h5, #contentArea .H5 {color:#018;}
.c3, #contentArea h1, #contentArea .H1, #contentArea h2, #contentArea .H2, #contentArea h3, #contentArea .H3, #contentArea h4, #contentArea .H4, #contentArea h6, #contentArea .H6 {color:#000;}
.c4, #contentArea .relatedLinksHead {color:#026;}
.c5, #chTB #chTer .item:hover, #chNav #chP a:hover, #chNav #chS a:hover, .pop a:hover {color:#0cc;}
.c6, #chNav #chPM a, #crumbBar a, #crumbBar a:hover, #contentArea a, #contentArea a:hover, #contentArea .dirTagLink, #contentArea #dedlM button {color:#16f;}
.c7, .lNavVertical a, .lNavHorizontal a,.lNavVertical a:hover, .lNavHorizontal a:hover,.lNavVertical a:visited, .lNavHorizontal a:visited, .lNavVerticalTabs a, .lNavHorizontalTabs a,.lNavVerticalTabs a:hover, .lNavHorizontalTabs a:hover,.lNavVerticalTabs a:visited, .lNavHorizontalTabs a:visited {color:#16f!important;}
.c9, .versal #versalBtm a, .versal #versalBtm a:hover, #chTB #chSearch #cst.sel, #chNav #chP td.sel a, #chNav #chS li a.sel, #chNav #chS li a.sel:hover, #chNav #chPM, #contentArea, #contentArea .smallText, #contentArea .largeText, .pubD #contentArea td, .pubD #contentArea td.heading, #footer a, .pop a {color:#222;}
.c11, #contentArea .title, .versal .date, #chNav #chP a, #chNav #chS a, #contentArea font.ImageBlock, span.ImageBlock, #contentArea .byLine, #contentArea .rssM .date {color:#666;}
.c2, #contentArea .rssM .publisher {color:#7a2;}
.c13, #contentArea a:visited {color:#808;}
.c17, #chTB #chTer .item, #crumbBar, #contentArea .subTitle, #contentArea .copyright {color:#999;}
.c18, #chTB #chSearch input[type="text"], #chTB #chSearch #cst {color:#bbb;}
.c19, #footer a:hover {color:#cff;}
.c20, .cr, .pop .h {color:#fff;}


/* backgrounds */

.bgc1, body {background-color: #acc;}
.bgc2, .pop .h {background-color:#999;}
.bgc3, .versal #zone1 div.infographic h5 {background-color:#dce6fa;}
.bgc4, .people .person .BlankPictureDiv {background-color:#eee;}
.bgc5, #shadow #top {background-color:#f3fafb;}
.bgc6, #border, .pop {background-color:#fff;}
.bgc7, hr {background-color:#ddd;}
.bgi1, body {background-image:url(/a/i/c/bg.gif);}
.bgi2, #chNav #chS, #chNav #chPM, #chNav #chP td.sel {background-image:url(/a/i/c/cover.png);}
.bgi3, #chNav {background-image:url(/a/i/c/grad.png);}
.bgi4, #bGrad {background-image:url(/a/i/c/grad3.gif);}
.bgi5, #crumbBar {background-image:url(/a/i/c/s_bc.png);}
.bgi6, #footer {background-image:url(/a/i/c/s_btm.png);}
.bgi7, #shadow {background-image:url(/a/i/c/s_mid.png);}
.bgi8, #chTB #chTer .item.t1:hover {background-image:url(/a/i/c/ter/h_downloads.gif);}
.bgi9, #chTB #chTer .item.t2:hover {background-image:url(/a/i/c/ter/h_papers.gif);}
.bgi10, #chTB #chTer .item.t3:hover {background-image:url(/a/i/c/ter/h_people.gif);}
.bgi11, #chTB #chTer .item.t4:hover {background-image:url(/a/i/c/ter/h_projects.gif);}
.bgi12, #chTB #chTer .item.t5:hover {background-image:url(/a/i/c/ter/h_video.gif);}
.bgi13, #chTB #chTer .item.t1 {background-image:url(/a/i/c/ter/n_downloads.gif);}
.bgi14, #chTB #chTer .item.t2 {background-image:url(/a/i/c/ter/n_papers.gif);}
.bgi15, #chTB #chTer .item.t3 {background-image:url(/a/i/c/ter/n_people.gif);}
.bgi16, #chTB #chTer .item.t4 {background-image:url(/a/i/c/ter/n_projects.gif);}
.bgi17, #chTB #chTer .item.t5 {background-image:url(/a/i/c/ter/n_video.gif);}
.bgi18, #contentArea #dedlM button:hover {background-image:url(/a/i/h_btn_dl.gif);}
.bgi19, #contentArea #dedlM button {background-image:url(/a/i/n_btn_dl.gif);}
.bgi20, .versal #zone2.conM, .gradTop, #contentArea #dedlM table.outer td.left, #contentArea #dedlM table.outer td.right, #contentArea #dedlM div.btm, .lNavVerticalTabs li, .lNavHorizontalTabs li {background-image:url(/apps/dp/i/shade_dn.png);}
.bgp1, #chTB #chTer .item.t1, #chTB #chTer .item.t1:hover, #chTB #chTer .item.t2, #chTB #chTer .item.t2:hover, #chTB #chTer .item.t3, #chTB #chTer .item.t3:hover, #chTB #chTer .item.t4, #chTB #chTer .item.t4:hover, #chTB #chTer .item.t5, #chTB #chTer .item.t5:hover {background-position:top center;}
.bgp2, .versal #zone2.conM {background-position:bottom;}
.bgr1, #footer, #contentArea .videoM .tile div:first-child, #contentArea .videoM .tileExtra div:first-child, #contentArea .videoM .ImageBlock, #contentArea .videoM .SmallImageBlock, #chTB #chTer .item.t1, #chTB #chTer .item.t1:hover, #contentArea #dedlM button, #contentArea #dedlM button:hover, #chTB #chTer .item.t2, #chTB #chTer .item.t2:hover, #chTB #chTer .item.t3, #chTB #chTer .item.t3:hover, #chTB #chTer .item.t4, #chTB #chTer .item.t4:hover, #chTB #chTer .item.t5, #chTB #chTer .item.t5:hover {background-repeat:no-repeat;}
.bgr2, body, .gradTop, .versal #zone2.conM, #crumbBar, #contentArea #dedlM table.outer td.left, #contentArea #dedlM table.outer td.right, #contentArea #dedlM div.btm, .lNavVerticalTabs li, .lNavHorizontalTabs li {background-repeat:repeat-x;}
.bg1, #contentArea #dedlM table.inner td.left, #contentArea #dedlM table.inner td.right, .lNavHorizontalTabs li.sel {background:none;}


/* borders */
.bc1, #contentArea .conM table {border-collapse:collapse;}
.bd2, .pop {border:1px solid #000;}
.bd3, .versal #zone1 div.infographic, .people .person img, #contentArea #dedlM table.outer {border:1px solid #999;}
.bd4, #contentArea .contentModule .BorderedImageWrapper, .conM .BorderedImageWrapper {border:1px solid #999 !important;}
.bd5, #border, #chTB #chSearch input[type="text"], #chTB #chSearch #cst, #chTB #chSearch #cst.sel {border:1px solid #cff;}
.bd6, #chNav #chP td.sel {border:1px solid #fff;}
.bdc1, .borderDarkColor {border-color:#999 !important;}
.bdc2, .borderLightColor {border-color:#ddd !important;}
.bdc2, table[borderColor="#ccccbb"] {border-color:#ccb !important;}
.bdc2, table[borderColor="#ddeeee"] {border-color:#dee !important;}
.bdt1, .borderTop {border-top: solid 1px;}
.bdt2, .gradTop {border-top:1px solid #999;}
.bdt3, #chTB #chSearch input[type="text"], #chTB #chSearch #cst {border-top:1px solid #b6b6af;}
.bdt4, #contentArea #dedlM table.inner td.left, #contentArea #dedlM table.inner td.right, .lNavVertical li:first-child, .lNavVerticalTabs li:first-child, .lNavHorizontalTabs li {border-top:1px solid #ccc;}
.bdt5, .bt, #crumbBar {border-top:1px solid #cff;}
.bdt6, #border, #chNav #chPM {border-top:1px solid #fff;}
.bdr1, .borderRight {border-right: solid 1px ;}
.bdr2, #footer li.last {border-right:0px transparent;}
.bdr3, #crumbBar #tools li.last {border-right:0px transparent;}
.bdr4, #crumbBar #tools li {border-right:1px solid #666;}
.bdr5, #footer li {border-right:1px solid #8e9b6b;}
.bdr6, ul.horiz li, #chNav #chP td.sel, #chNav #chS {border-right:1px solid #bbb;}
.bdr7, .lNavVerticalTabs li, .lNavHorizontalTabs li {border-right:1px solid #ccc;}
.bdr8 {border-right:none;}
.bdr9, ul.horiz li.last {border-right:transparent;}
.bdb1, .borderBottom {border-bottom: solid 1px;}
.bdb2, .pop .h {border-bottom:1px solid #000;}
.bdb3, #contentArea h1.rule, #contentArea .H1.rule, #contentArea h2.rule, #contentArea .H2.rule {border-bottom:1px solid #998;}
.bdb4, .versal #zone2 div {border-bottom:1px solid #999;}
.bdb5, .lNavVertical li, .lNavVerticalTabs li, .lNavHorizontalTabs li {border-bottom:1px solid #ccc;}
.bdb6, .bb {border-bottom:1px solid #cff;}
.bdb7, #chNav #chP td {border-bottom:1px solid #fff;}
.bdb8, #chNav #chP td.sel, .lNavHorizontalTabs li.sel {border-bottom:none;}
.bdl1, .borderLeft {border-left: solid 1px ;}
.bdl2, #footer li.first {border-left:0px transparent;}
.bdl3, .versal #zone2 div, #contentArea #dedlM table.outer > tbody > tr > td.right {border-left:1px solid #999;}
.bdl4, #chTB #chSearch input[type="text"], #chTB #chSearch #cst {border-left:1px solid #b6b6af;}
.bdl5, .lNavVerticalTabs li, .lNavHorizontal li, .lNavHorizontalTabs li:first-child {border-left:1px solid #ccc;}
.bdl6, ul.horiz li, #chNav #chPM, #footer li {border-left:1px solid #fff;}
.bdl7, #crumbBar #tools li {border-left:none;}
.bdl8, ul.horiz li.first, .lNavHorizontal li:first-child {border-left:transparent;}
.bd1, #chTB #chLogo img, #chNav #chPM img, #contentArea #dedlM button, #contentArea span.ImageBlock img, font.ImageBlock img, span.ImageBlock, font.ImageBlock, hr {border:none;}


/* line height, word wrap, and letter spacing */
.lh1, #contentArea .peMi .item a, #contentArea .peMi .item span, #contentArea .rssM td ul
.lh2,  #contentArea h5, #contentArea .H5, #contentArea .peMi .item .byLine {line-height:1.25;}
.lh3, #chNav #chPM, #contentArea .conM li, #contentArea p, #contentArea td, #contentArea .byLine, #contentArea .copyright, #contentArea .smallText, #contentArea .largeText {line-height:1.5;}
.lh4, #contentArea #dedlM table.outer td, #contentArea .rssM .date {line-height:normal;}
.ww1, #contentArea #dedM, #contentArea #dpeM, #contentArea font.ImageBlock, span.ImageBlock, #contentArea .conM {word-wrap:break-word;}
.lsp1, #contentArea .relatedLinksHead {letter-spacing:1px;}


/* margins paddings */
.mt2 {margin-top:-10px;}
.mt3, #contentArea .rssM p+.date {margin-top:-14px;}
.mt4, *, .fw #contentArea .conM ul ul ul, #contentArea .conM ul ol, #contentArea .conM ol ul, .center, ul.horiz, .versal #versalBtm, #border, #crumbBar #tools img, #contentArea .deM, #contentArea #dedlM table.inner form, #contentArea .peMi .item, contentArea .peMi .itemShort, #contentArea .rssM td img, #contentArea td p, #contentArea .videoM .tile, #contentArea .videoM .tileExtra, #contentArea .videoM .SmallImageBlock img, #contentArea .videoM p, .medMargin, .people .person, .pop .h, #contentArea .conM ul, #contentArea .conM ol, #contentArea .conM li, #contentArea p, .lNavHorizontal ul, .lNavHorizontalTabs ul, #contentArea .conM p+ol, #contentArea .conM p+ul {margin-top:0px;}
.mt5, #contentArea .videoM .ImageBlock img  {margin-top:0px !important;}
.mt6, .pop ul li {margin-top:3px;}
.mt7, #contentArea .pubsM > ul > li > .smallText, #contentArea #dedlM button, #contentArea .rssM .date, #footer ul {margin-top:4px;}
.mt8, #chNav #chS li {margin-top:5px;}
.mt9, .mSmallTop, #contentArea .conM ul ul, #contentArea .videoM .date+p, .versal .title, .pubD .title, .versal #zone1 div.embeddedVideo, .versal #zone1 div.imageFloatLeft, .versal #zone1 div.imageFloatRight, .fw #contentArea .deM, #contentArea #dedM img, #contentArea #dpeM, .versal #zone1 div.infographic, div.lNavHorizontal, div.lNavHorizontalTabs, .lNavVerticalTabs ul {margin-top:6px;}
.mt10, #contentArea .title {margin-top:6px !important;}
.mt17, hr {margin-top:7px;}
.mt11 {margin-top:8px;}
.mt12, .mMedTop {margin-top:12px;}
.mt13, body {margin-top:16px;}
.mt14, .mLargeTop, #contentArea #dedlM table.inner {margin-top:18px;}
.mt15, .mXlargeTop, #contentArea #dedlM table.outer td.right p {margin-top:21px;}
.mt16, .versal #zone1.conM, .versal #zone2.conM {margin-top:25px;}
.mr1, #contentArea #dedlM button {margin-right:-3px;}
.mr2, *, body, ul.horiz, .versal #versalBtm, #contentArea #dedlM table.inner form, #contentArea td p, #contentArea .videoM p, .pop .h, #contentArea .conM ul, #contentArea .conM ol, #contentArea .conM li, #contentArea p, .versal #zone1 div.imageFloatRight, .lNavHorizontal ul, .lNavHorizontalTabs ul {margin-right:0px;}
.mr3, #contentArea .videoM .ImageBlock img {margin-right:0px !important;}
.mr4, #crumbBar #tools img {margin-right:2px;}
.mr5, .pop ul li {margin-right:5px;}
.mr6, .mSmallRight, .versal #zone1 div.embeddedVideo, .fw #contentArea .deM, .versal #zone1 div.infographic {margin-right:6px;}
.mr7, .versal #zone1 img.inlineImageleft, #footer img, #contentArea .rssM td img {margin-right:10px;}
.mr8, #border {margin-right:11px;}
.mr9, .mMedRight, #contentArea #dpeM img, #contentArea .peMi .item, #contentArea .peMi .itemShort, .medMargin {margin-right:12px;}
.mr10, #contentArea .videoM .SmallImageBlock img, #contentArea #dedM img, #contentArea .videoM .ImageBlock {margin-right:15px;}
.mr11, .mLargeRight, #contentArea .deM, .versal #zone1 div.imageFloatLeft, #contentArea #dpeM {margin-right:18px;}
.mr12, .prjm img {margin-right:20px;}
.mr13, .mXlargeRight {margin-right:21px;}
.mr14, .people .person {margin-right:30px;}
.mr15, .versal #zone1.conM {margin-right:36px;}
.mr16, #contentArea .videoM .tile, #contentArea .videoM .tileExtra  {margin-right:42px;}
.mr17, #footer span {margin-right:68px;}
.mr18, .center {margin-right:auto;}
.mb1, *, body, .center, #contentArea .conM ol ol, #contentArea .conM ul ol, #contentArea #dedM img+p, ul.horiz, #border, #crumbBar #tools img, #contentArea .deM, #contentArea #dedlM table.inner form, #contentArea .rssM td img, #contentArea td p, .medMargin, .people .person, .pop .h, .versal #zone1.conM, .versal #zone1 div.embeddedVideo, .versal #zone1 div.infographic, #contentArea .videoM .SmallImageBlock, .lNavHorizontal ul, .lNavHorizontalTabs ul {margin-bottom:0px;}
.mb2, #contentArea .videoM .ImageBlock img {margin-bottom:0px !important;}
.mb3, #contentArea h1.rule, #contentArea .H1.rule, #contentArea h2.rule, #contentArea .H2.rule, .pop ul li {margin-bottom:3px;}
.mb4, .mSmallBottom, .versal #zone1 div.infographic h5, .fw #contentArea .conM ul ul, #contentArea .conM ul ul, #contentArea .conM ol ul, #contentArea .conM li {margin-bottom:6px;}
.mb13, hr {margin-bottom:7px;}
.mb5, .people .manager, .versal #zone1 div.imageFloatLeft, .versal #zone1 div.imageFloatRight {margin-bottom:10px;}
.mb6, .mMedBottom, #contentArea font.ImageBlock, #contentArea .peMi .item, #contentArea .peMi .itemShort, .fw #contentArea .deM, #contentArea #dpeM, span.ImageBlock {margin-bottom:12px;}
.mb7, .versal .title, .pubD .title {margin-bottom:14px !important;}
.mb8, #contentArea .videoM .SmallImageBlock img {margin-bottom:15px;}
.mb9, .mLargeBottom, #contentArea h6, #contentArea .H6, #contentArea .subTitle, #contentArea .videoM .tile, #contentArea .videoM .tileExtra, #contentArea .videoM p, #contentArea .conM ul, #contentArea .conM ol, #contentArea p, #contentArea #dedM, #contentArea #dedM img, #contentArea #dpeM img, .lNavVerticalTabs ul {margin-bottom:18px;}
.mb10, #contentArea .title {margin-bottom:18px !important;}
.mb11, .mXlargeBottom {margin-bottom:21px;}
.mb12, .versal #versalBtm, div.lNavHorizontal, div.lNavHorizontalTabs {margin-bottom:27px;}
.ml1, #contentArea #dedlM button {margin-left:-3px;}
.ml2, *, body, .versal #versalBtm img#iBtt, .versal #versalBtm td:first-child img, ul.horiz, .versal #versalBtm, #contentArea #dedlM table.inner form, #contentArea .peMi .item, #contentArea .peMi .itemShort, #contentArea .rssM td img, #contentArea td p, #contentArea .videoM .tile, #contentArea .videoM .tileExtra, #contentArea .videoM .SmallImageBlock img, #contentArea .videoM p, .people .person, .pop .h, #contentArea .conM ul, #contentArea .conM ol, #contentArea .conM li, #contentArea p, .versal #zone1.conM, .versal #zone1 div.embeddedVideo, .versal #zone1 div.imageFloatLeft, #contentArea #dedM img, .versal #zone1 div.infographic, .lNavHorizontal ul, .lNavHorizontalTabs ul {margin-left:0px;}
.ml3, #contentArea .videoM .ImageBlock img {margin-left:0px !important;}
.ml4, #crumbBar #tools img {margin-left:2px;}
.ml5, .pop ul li {margin-left:5px;}
.ml6, .mSmallLeft {margin-left:6px;}
.ml7, .versal #zone1 img.inlineImageright, .versal #zone1 div.imageFloatRight {margin-left:10px;}
.ml8, #border {margin-left:11px;}
.ml9, .mMedLeft, .fw #contentArea .deM, .fw div.lNavHorizontal, .fw div.lNavHorizontalTabs {margin-left:12px;}
.ml10, #contentArea .conM blockquote, #footer ul {margin-left:15px;}
.ml11, .mLargeLeft, #contentArea .deM, .medMargin, #contentArea #dpeM, div.lNavHorizontal, div.lNavHorizontalTabs {margin-left:18px;}
.ml12, .mXlargeLeft {margin-left:21px;}
.ml13, .versal #versalBtm img {margin-left:27px;}
.ml14, .center {margin-left:auto;}



.pt1, .versal #zone2 div:first-child, #footer li, .w, .project1 #zone3, .versal #zone1 div.infographicInner, .versal #zone2.conM, .people, #chNav #chS li, #crumbBar #tools li, #crumbBar #tools li.last, .fw #contentArea .conM ul ul ul, #contentArea .conM, #contentArea .conM ul ul, #contentArea .conM ol ul, #contentArea h2, #contentArea .H2, #contentArea h3, #contentArea .H3, #contentArea h4, #contentArea .H4, #contentArea h5, #contentArea .H5, #contentArea .videoM .SmallImageBlock, .versal #zone1.conM, .versal #zone1 div.infographic, .people .person, #contentArea .conM ul, #contentArea .conM ol, #contentArea .conM li, #contentArea p, .lNavHorizontal ul, .lNavHorizontalTabs ul {padding-top:0;}
.pt2, .fw #contentArea .title+.compositeModule_2_1Zone  > .zone > .conM:first-child {padding-top:0 !important;}
.pt3, #chSearch input[type="text"], #chSearch #cst {padding-top:1px;}
.pt4, .lNavHorizontal li {padding-top:2px;}
.pt5, .versal #zone1 div.infographic h5, .pop .h {padding-top:3px;}
.pt6, #footer {padding-top:5px;}
.pt7, #chNav #chP td.sel div, .versal #zone2 div, #crumbBar, .lNavVertical li, .lNavVerticalTabs li, .lNavHorizontalTabs li, div.lNavHorizontal, div.lNavHorizontalTabs {padding-top:6px;}
.pt8, #chNav #chP td div, #contentArea #dedlM table.inner td {padding-top:9px;}
.pt9, #contentArea {padding-top:10px;}
.pt10, .fw #contentArea .conM {padding-top:12px;}
.pt11, #contentArea #dedlM table.outer > td {padding-top:24px;}
.pt12, #chTer .item {padding-top:36px;}
.pt13, .medMargin, .project1 #zone1, .project1 #zone2 {padding-top:50px;}
.pr1, .versal #zone1 div.infographic h5, .versal #zone2.conM, .versal #zone2 div, .people, .fw #contentArea .conM ul ul ul, #contentArea h2, #contentArea .H2, #contentArea h3, #contentArea .H3, #contentArea h4, #contentArea .H4, #contentArea h5, #contentArea .H5, #contentArea #dedlM table.inner td, .lNavVertical li, .lNavVerticalTabs li, #contentArea .videoM .SmallImageBlock, .versal #zone1.conM, .versal #zone1 div.infographic, .people .person, #contentArea .conM ul, #contentArea .conM ol, #contentArea .conM li, #contentArea p, .lNavHorizontal ul, .lNavHorizontalTabs ul {padding-right:0;}
.pr2, #footer li {padding-right:1em;}
.pr3, #crumbBar #tools li.last, .pop .h {padding-right:3px;}
.pr4, .versal #zone1 div.infographicInner, #crumbBar, .fw #contentArea {padding-right:6px;}
.pr5, #crumbBar #tools li {padding-right:9px;}
.pr6, .fw #contentArea .conM, .w, .lNavHorizontal li, .lNavHorizontalTabs li {padding-right:12px;}
.pr7, #chNav #chS li {padding-right:15px;}
.pr8, #chNav #chP td div, #contentArea .conM, #contentArea .conM ul ul, #contentArea .conM ol ul {padding-right:18px;}
.pr9, #contentArea {padding-right:19px;}
.pr10, #contentArea #dedlM table.outer > td {padding-right:24px;}
.pr11, .project1 #zone1, .project1 #zone2, .project1 #zone3 {padding-right:50px;}
.pb1, #contentArea .videoM td, #footer li, .w, .project1 #zone1, .project1 #zone2, .versal #zone1 div.infographicInner, .versal #zone2 div, .people, #chNav #chS li, #crumbBar, #crumbBar #tools li, #crumbBar #tools li.last, #contentArea, #contentArea .conM, #contentArea .conM ul ul, #contentArea .conM ol ul, #contentArea .videoM .SmallImageBlock, .versal #zone1.conM, .versal #zone1 div.infographic, #contentArea .conM ul, #contentArea .conM ol, #contentArea .conM li, #contentArea p, .lNavHorizontal ul, .lNavHorizontalTabs ul {padding-bottom:0;}
.pb2, #chNav #chP td.sel div, .versal #zone1 div.infographic h5, #chNav #chP td div, .lNavHorizontal li, .pop .h {padding-bottom:3px;}
.pb3, #contentArea h1.rule, #contentArea .H1.rule, #contentArea h2.rule, #contentArea .H2.rule {padding-bottom:4px;}
.pb4, .prjm .title {padding-bottom:5px;}
.pb5, .fw #contentArea, .fw #contentArea .conM ul ul ul, #contentArea h3, #contentArea .H3, #contentArea h4, #contentArea .H4, .lNavHorizontalTabs li {padding-bottom:6px;}
.pb6, .lNavVertical li, .lNavVerticalTabs li {padding-bottom:7px;}
.pb7, #contentArea #dedlM table.inner td {padding-bottom:9px;}
.pb8, .project1 #zone3, #contentArea h5, #contentArea .H5 {padding-bottom:10px;}
.pb9, #contentArea h2, #contentArea .H2 {padding-bottom:12px;}
.pb10, #contentArea h1, #contentArea .H1 {padding-bottom:15px;}
.pb11, #contentArea .rssM td, .lNavVertical ul {padding-bottom:18px;}
.pb12, .people .person {padding-bottom:20px;}
.pb13, #contentArea #dedlM table.outer > td {padding-bottom:24px;}
.pb14, .prjm, .versal #zone2.conM {padding-bottom:25px;}
.pb15 {padding-bottom:11px;}
.pl1, ul.horiz, .lNavHorizontal li:first-child, #footer .first, .project1 #zone1, .versal #zone2.conM, .fw #contentArea .conM ul ul ul, #contentArea h2, #contentArea .H2, #contentArea h3, #contentArea .H3, #contentArea h4, #contentArea .H4, #contentArea h5, #contentArea .H5, #contentArea #dedlM table.inner td, .lNavVertical li, #contentArea .videoM .SmallImageBlock, .versal #zone1.conM, .versal #zone1 div.infographic, .people .person, #contentArea .conM li, #contentArea p, .lNavHorizontal ul, .lNavHorizontalTabs ul {padding-left:0;}
.pl2, #footer li {padding-left:1em;}
.pl3, .versal #zone1 div.infographic h5, .pop .h {padding-left:3px;}
.pl4, #crumbBar #tools li.last {padding-left:5px;}
.pl5, #chSearch input[type="text"], #chSearch #cst, .versal #zone1 div.infographicInner, #crumbBar, .fw #contentArea {padding-left:6px;}
.pl6, #crumbBar #tools li {padding-left:8px;}
.pl7, .versal #zone2 div {padding-left:10px;}
.pl8, .fw #contentArea .conM, .w, .lNavVerticalTabs li, .lNavHorizontal li, .lNavHorizontalTabs li {padding-left:12px;}
.pl9, .people {padding-left:14px;}
.pl10, #chNav #chS li {padding-left:15px;}
.pl11, #chNav #chP td div, #contentArea .conM, #contentArea .conM ul ul, #contentArea .conM ol ul, #contentArea .conM ul, .lNavVertical ul, .lNavVerticalTabs ul {padding-left:18px;}
.pl12, #contentArea #dedlM table.outer > td {padding-left:24px;}
.pl13, #contentArea .conM ol {padding-left:28px;}
.pl14, .project1 #zone2, .project1 #zone3 {padding-left:50px;}
.pl15, #contentArea {padding-left:56px;}


/* lists */
.lst1, .pop ul li {list-style-type:circle;}
.lst2, #contentArea .conM ol ol ol ol {list-style-type:lower-alpha;}
.lst3, #contentArea .conM ol ol ol {list-style-type:lower-roman;}
.lst4, ul.horiz li, .lNavVertical ul, .lNavVerticalTabs ul, .lNavHorizontal ul, .lNavHorizontalTabs ul {list-style-type:none;}
.lst5, #contentArea .conM ul {list-style-type:disc;}
.lst6, #contentArea .conM ol ol, #contentArea .conM ul ol {list-style-type:upper-alpha;}

/* floats and positioning */

.cb, .people .b {clear:both;}
.cl {clear:left;}
.cr {clear:right;}
/* .FR .FL .FN  being kept for legacy purposes of existing pages already using this class */
.fl, .FL, .prjm img, ul.horiz li, .project1 #zone3, .versal #zone1.conM, .versal #zone1 div.embeddedVideo, .versal #zone1 div.imageFloatLeft, .versal #zone1 div.infographic, .versal #zone2.conM, .people .person, .compositeModule_2Zone > div.zone, .compositeModule_3Zone > div.zone, .compositeModule_4Zone > div.zone, .compositeModule_1_2Zone > div.zone:first-child, .compositeModule_1_2Zone > div.zone + div.zone, .compositeModule_2_1Zone > div.zone:first-child, .compositeModule_2_1Zone > div.zone + div.zone, .compositeModule_1_3Zone > div.zone:first-child, .compositeModule_1_3Zone > div.zone + div.zone, .compositeModule_3_1Zone > div.zone:first-child, .compositeModule_3_1Zone > div.zone + div.zone, .compositeModule_1_2_1Zone > div.zone:first-child, .compositeModule_1_2_1Zone > div.zone + div.zone + div.zone, .compositeModule_1_2_1Zone > div.zone + div.zone, .fw .compositeModule_3Zone > div.zone + div.zone, .fw .compositeModule_3Zone > div.zone + div.zone + div.zone, #contentArea .peMi .item, #contentArea .peMi .itemShort, #contentArea .videoM .tile, #contentArea .videoM .tileExtra {float:left;}
.fr, .FR, .project1 #zone1, .versal #zone1 div.imageFloatRight {float:right;}

.pa, #shadow #top, #chTB #chLogo, #chTB #chSearch, #chTB #chSearch div, #chTB #chSearch input[type="text"], #chTB #chSearch #cst, #chTB #chTer, #chNav #chP, #chNav #chS, #chNav #chPM, #crumbBar #tools, .pop {position:absolute;}
.pr, .versal #versalBtm, #shadow, #border, #chNav, #crumbBar {position:relative;}

.r1, #crumbBar #tools {right:0px;}
.t1, #chTB #chLogo, #chTB #chSearch input[type="text"], #chTB #chSearch #cst, #chNav {top:0px;}
.t2, #chTB #chTer {top:3px;}
.t3, #chNav #chP, #chNav #chPM {top:7px;}
.t4, #chTB #chSearch {top:18px;}
.t5, #chTB #chSearch div {top:24px;}
.t6, #chNav #chS {top:37px;}
.t7, #cShare {top:170px;}
.l1, #chNav, #chNav #chP, #chTB #chSearch div, #chTB #chSearch input[type="text"], #chTB #chSearch #cst, #chNav #chS, #shadow #top {left:0px;}
.l2, #chTB #chLogo {left:12px;}
.l3, #chTB #chSearch {left:258px;}
.l4, #chTB #chSearch #goButton {left:302px;}
.l5, #chTB #chTer {left:627px;}
.l6, #chNav #chPM {left:653px;}
.l7, #cShare {left:850px;}

.zi1, #chNav #chS {z-index:1;}
.zi2, #chNav #chP {z-index:2;}
.zi3, #shadow {z-index:5;}
.zi4, #shadow #top {z-index:6;}
.zi5, .pop, #border {z-index:10;}


/* display */
.dib, #bcHolder, .fn, .FN {display:inline-block;}
.dn {display:none;}
.db, .cl {display:block;}
.din, .lNavHorizontal li, .lNavHorizontalTabs li {display:inline;}
.oh, .zone, .project1 .zone, #chTer, #chNav #chS, #bcHolder, #contentArea .videoM .tile, #contentArea .videoM .tileExtra {overflow:hidden;}
.vh, .cl {visibility:hidden;}
.ws2, .versal #versalBtm td p, #bcHolder, #chNav #chP td div {white-space:nowrap;}

.z1, #contentArea font.ImageBlock, span.ImageBlock {zoom:1;}
.wdsp1, #contentArea h5, #contentArea .H5 {word-spacing: -0.05em;}
.wdsp2, .lNavHorizontal ul, .lNavHorizontalTabs ul {word-spacing:-5px;}
.wdsp3, .lNavHorizontal li, .lNavHorizontalTabs li {word-spacing:normal;}

 .content, .cl {content:".";}
.black-and-white {}
.gray-stripe {border-color: #666 !important;}
.teal-stripe {border-color: #4D8C8C !important;}
.blue-stripe {border-color: #369 !important;}
.blue {border-color: #FFF !important;}
 
/* Classic Black and White */
.black-and-white tr.black-and-whiteTableHeaderRow {background-color: Black; color: #FFF; } 
.black-and-white tr.black-and-whiteTableHeaderRow th {font-weight: bold; } 
.black-and-white tr.black-and-whiteTableHeaderRow td {font-weight: bold; } 
.black-and-white td.black-and-whiteTableHeaderFirstCol {border-left: solid 1px black; border-right: solid 2px black !important; font-weight: bold;} 
.black-and-white td.black-and-whiteTableHeaderLastCol {font-weight: bold; border-right: 1px solid black;} 
.black-and-white td.black-and-whiteTableHeaderOddCol {} 
.black-and-white td.black-and-whiteTableHeaderEvenCol {} 

.black-and-white tr.black-and-whiteTableOddRow {} 
.black-and-white tr.black-and-whiteTableEvenRow {} 
.black-and-white td.black-and-whiteTableFirstCol {border-left: solid 1px black; border-right: solid 2px black !important; font-weight: bold;} 
.black-and-white th.black-and-whiteTableFirstCol {border-left: solid 1px black; border-right: solid 2px black !important; font-weight: bold;} 
.black-and-white td.black-and-whiteTableLastCol {border-left: 1px solid black; border-right: solid 1px black; font-weight: bold;} 
.black-and-white th.black-and-whiteTableLastCol {border-left: 1px solid black; border-right: solid 1px black; font-weight: bold;} 
.black-and-white td.black-and-whiteTableOddCol {} 
.black-and-white td.black-and-whiteTableEvenCol {} 

.black-and-white tr.black-and-whiteTableFooterRow {font-weight: bold;} 
.black-and-white tr.black-and-whiteTableFooterRow td {border-bottom: solid 1px black; border-top: 1px solid black;} 
.black-and-white td.black-and-whiteTableFooterFirstCol {border-left: 1px solid black; border-right: solid 2px black !important; font-weight: bold;} 
.black-and-white td.black-and-whiteTableFooterLastCol {font-weight: bold; border-right: solid 1px black; border-left: 1px solid black;} 
.black-and-white td.black-and-whiteTableFooterOddCol {} 
.black-and-white td.black-and-whiteTableFooterEvenCol {} 

.black-and-white th {font-weight: normal;}


/* Classic Grayscale Zebra */
.gray-stripe tr.gray-stripeTableHeaderRow {background-color: #666; color: #FFF; } 
.gray-stripe tr.gray-stripeTableHeaderRow th {font-weight: bold; } 
.gray-stripe tr.gray-stripeTableHeaderRow td {font-weight: bold; } 
.gray-stripe td.gray-stripeTableHeaderFirstCol {border-left: solid 1px #666 !important; border-right: solid 2px #666 !important; font-weight: bold;} 
.gray-stripe td.gray-stripeTableHeaderLastCol {font-weight: bold; border-right: 1px solid #666 !important;} 
.gray-stripe td.gray-stripeTableHeaderOddCol {} 
.gray-stripe td.gray-stripeTableHeaderEvenCol {} 

.gray-stripe tr.gray-stripeTableOddRow {} 
.gray-stripe tr.gray-stripeTableEvenRow {background-color: #eee;} 
.gray-stripe td.gray-stripeTableFirstCol {border-left: solid 1px #666 !important; border-right: solid 2px #666 !important; font-weight: bold;} 
.gray-stripe th.gray-stripeTableFirstCol {border-left: solid 1px #666 !important; border-right: solid 2px #666 !important; font-weight: bold;} 
.gray-stripe td.gray-stripeTableLastCol {border-left: 1px solid #666 !important; border-right: solid 1px #666 !important; font-weight: bold;} 
.gray-stripe th.gray-stripeTableLastCol {border-left: 1px solid #666 !important; border-right: solid 1px #666 !important; font-weight: bold;} 
.gray-stripe td.gray-stripeTableOddCol {} 
.gray-stripe td.gray-stripeTableEvenCol {} 

.gray-stripe tr.gray-stripeTableFooterRow {font-weight: bold;}
.gray-stripe tr.gray-stripeTableFooterRow td {border-top: 3px solid #666 !important; border-bottom: 2px solid #666 !important;} 
.gray-stripe td.gray-stripeTableFooterFirstCol {border-left: 1px solid #666 !important; border-right: solid 2px #666 !important; font-weight: bold;} 
.gray-stripe td.gray-stripeTableFooterLastCol {border-left: 1px solid #666 !important; border-right: solid 1px #666 !important; font-weight: bold;} 
.gray-stripe td.gray-stripeTableFooterOddCol {} 
.gray-stripe td.gray-stripeTableFooterEvenCol {} 

.gray-stripe th {font-weight: normal;}
.gray-stripe td {border-color: #666 !important; }
.gray-stripe th {border-color: #666 !important; }

/* Simple Teal Zebra */
.teal-stripe tr.teal-stripeTableHeaderRow {background-color: #4D8C8C; color: #FFF;} 
.teal-stripe tr.teal-stripeTableHeaderRow th {font-weight: bold; border-top: 1px solid #4D8C8C !important; border-bottom: 1px solid #4D8C8C !important; } 
.teal-stripe tr.teal-stripeTableHeaderRow td {font-weight: bold; border-top: 1px solid #4D8C8C !important; border-bottom: 1px solid #4D8C8C !important;} 
.teal-stripe td.teal-stripeTableHeaderFirstCol {border-left: solid 1px #4D8C8C !important; border-right: solid 2px #4D8C8C !important; font-weight: bold;} 
.teal-stripe td.teal-stripeTableHeaderLastCol {font-weight: bold; border-left: 1px solid #4D8C8C !important; border-right: 1px solid #4D8C8C !important;} 
.teal-stripe td.teal-stripeTableHeaderOddCol {} 
.teal-stripe td.teal-stripeTableHeaderEvenCol {} 

.teal-stripe tr.teal-stripeTableOddRow {} 
.teal-stripe tr.teal-stripeTableEvenRow {background-color: #E8F0F0;} 
.teal-stripe td.teal-stripeTableFirstCol {border-left: solid 1px #4D8C8C !important; border-right: solid 2px #4D8C8C !important; font-weight: bold;} 
.teal-stripe th.teal-stripeTableFirstCol {border-left: solid 1px #4D8C8C !important; border-right: solid 2px #4D8C8C !important; font-weight: bold;} 
.teal-stripe td.teal-stripeTableLastCol {border-left: 1px solid #4D8C8C !important; border-right: solid 1px #4D8C8C !important; font-weight: bold;} 
.teal-stripe th.teal-stripeTableLastCol {border-left: 1px solid #4D8C8C !important; border-right: solid 1px #4D8C8C !important; font-weight: bold;} 
.teal-stripe td.teal-stripeTableOddCol {} 
.teal-stripe td.teal-stripeTableEvenCol {} 

.teal-stripe tr.teal-stripeTableFooterRow {font-weight: bold;} 
.teal-stripe tr.teal-stripeTableFooterRow td {border-top: 3px solid #4D8C8C !important; border-bottom: 2px solid #4D8C8C !important;} 
.teal-stripe td.teal-stripeTableFooterFirstCol {border-left: 1px solid #4D8C8C !important; border-right: solid 2px #4D8C8C !important; font-weight: bold;} 
.teal-stripe td.teal-stripeTableFooterLastCol {border-left: 1px solid #4D8C8C !important; border-right: solid 1px #4D8C8C !important;} 
.teal-stripe td.teal-stripeTableFooterOddCol {} 
.teal-stripe td.teal-stripeTableFooterEvenCol {} 

.teal-stripe th {font-weight: normal;}
.teal-stripe td {border-color: #4D8C8C !important; }
.teal-stripe th {border-color: #4D8C8C !important; }

/* Simple Blue Horizontal Zebra */
.blue-stripe tr.blue-stripeTableHeaderRow {background-color: #369; color: #FFF; } 
.blue-stripe tr.blue-stripeTableHeaderRow th {font-weight: bold; } 
.blue-stripe tr.blue-stripeTableHeaderRow td {font-weight: bold; } 
.blue-stripe td.blue-stripeTableHeaderFirstCol {border-left: solid 1px #369 !important; border-right: solid 2px #369 !important; font-weight: bold;} 
.blue-stripe td.blue-stripeTableHeaderLastCol {border-left: 1px solid #369 !important; border-right: 1px solid #369 !important; font-weight: bold; } 
.blue-stripe td.blue-stripeTableHeaderOddCol {} 
.blue-stripe td.blue-stripeTableHeaderEvenCol {} 

.blue-stripe tr.blue-stripeTableOddRow {} 
.blue-stripe tr.blue-stripeTableEvenRow {background-color: #E5EBF2;} 
.blue-stripe td.blue-stripeTableFirstCol {border-left: 1px solid #369 !important; border-right: solid 2px #369 !important; font-weight: bold;} 
.blue-stripe th.blue-stripeTableFirstCol {border-left: 1px solid #369 !important; border-right: solid 2px #369 !important; font-weight: bold;}
.blue-stripe td.blue-stripeTableLastCol {border-left: 1px solid #369 !important; border-right: solid 1px #369 !important; font-weight: bold;} 
.blue-stripe th.blue-stripeTableLastCol {border-left: 1px solid #369 !important; border-right: solid 1px #369 !important; font-weight: bold;}
.blue-stripe td.blue-stripeTableOddCol {} 
.blue-stripe td.blue-stripeTableEvenCol {} 

.blue-stripe tr.blue-stripeTableFooterRow {font-weight: bold;}
.blue-stripe tr.blue-stripeTableFooterRow td {border-top: 3px solid #369 !important; border-bottom: 2px solid #369 !important;} 
.blue-stripe td.blue-stripeTableFooterFirstCol {border-left: 1px solid #369 !important; border-right: solid 2px #369 !important; font-weight: bold;} 
.blue-stripe td.blue-stripeTableFooterLastCol {border-left: 1px solid #369 !important; border-right: solid 1px #369 !important; font-weight: bold;} 
.blue-stripe td.blue-stripeTableFooterOddCol {} 
.blue-stripe td.blue-stripeTableFooterEvenCol {} 

.blue-stripe th {font-weight: normal;}
.blue-stripe td {border-color: #369 !important; }
.blue-stripe th {border-color: #369 !important; }

/* Simple Blue */
.blue tr.blueTableHeaderRow {background-color: #C1D1E0;} 
.blue tr.blueTableHeaderRow th {font-weight: bold; } 
.blue tr.blueTableHeaderRow td {font-weight: bold; } 
.blue td.blueTableHeaderFirstCol {border-left: solid 1px #FFF !important; border-right: solid 2px #FFF !important; font-weight: bold;} 
.blue td.blueTableHeaderLastCol {border-left: 1px solid #FFF !important; border-right: 1px solid #FFF !important; font-weight: bold;} 
.blue td.blueTableHeaderOddCol {} 
.blue td.blueTableHeaderEvenCol {} 

.blue tr.blueTableOddRow {} 
.blue tr.blueTableEvenRow {} 
.blue td.blueTableFirstCol {border-left: 1px solid #FFF !important; border-right: solid 2px #FFF !important; font-weight: bold;} 
.blue th.blueTableFirstCol {border-left: 1px solid #FFF !important; border-right: solid 2px #FFF !important; font-weight: bold;} 
.blue td.blueTableLastCol {border-left: 1px solid #FFF !important; border-right: solid 1px #FFF !important; font-weight: bold;} 
.blue th.blueTableLastCol {border-left: 1px solid #FFF !important; border-right: solid 1px #FFF !important; font-weight: bold;} 
.blue td.blueTableOddCol {} 
.blue td.blueTableEvenCol {} 

.blue tr.blueTableFooterRow {font-weight: bold;}
.blue tr.blueTableFooterRow td {border-top: 3px solid #FFF !important; border-bottom: 2px solid #FFF !important;} 
.blue td.blueTableFooterFirstCol {border-left: 1px solid #FFF !important; border-right: solid 2px #FFF !important; font-weight: bold;} 
.blue td.blueTableFooterLastCol {border-left: 1px solid #FFF !important; border-right: solid 1px #FFF !important; font-weight: bold;} 
.blue td.blueTableFooterOddCol {} 
.blue td.blueTableFooterEvenCol {} 

.blue th {font-weight: normal;}
.blue tr {background-color: #E5EBF2;}
.blue td {border-bottom-color: #FFF !important; border-bottom-style: solid; border-bottom-width: 1px!important;}
.blue td {border-color: #FFF !important; }
.blue th {border-color: #FFF !important; }
#contentArea .conM table.tWiz { }
#contentArea .conM table.tWiz, #contentArea .conM table.tWiz td, #contentArea .conM table.tWiz th { border-color: #323223 }
#contentArea .conM table.tableBorder { border: solid 1px }
#contentArea .conM table.tableBorderTop    { border-top: solid 1px }
#contentArea .conM table.tableBorderBottom { border-bottom: solid 1px }
#contentArea .conM table.borderRows td, table.borderRows th { border-top: solid 1px; border-bottom: solid 1px;}
#contentArea .conM table.borderColumns td, table.borderColumns th { border-left: solid 1px; border-right: solid 1px;}
    
    </STYLE>
     
<SCRIPT type="text/javascript">
      var rmc = {
  b: {
    IE: (navigator.appName.toLowerCase() == "microsoft internet explorer"),
	V9:(navigator.appVersion.indexOf("MSIE 9") > -1),
    O: (typeof (window.opera) != "undefined")
  },
  Hovers: [],
  Fades: [],
  Xml: [],
  Xsl: [],
  MaxS: 0,
  GE: function(s) { return document.getElementById(s); },
  AE: function(o, e, r) {
    if (o == null) { return; }
    (this.b.IE) ? o.attachEvent("on" + e, r) : o.addEventListener(e, r, false);
  },
  RE: function(o, e, r) {
    if (o == null) { return; }
    (this.b.IE) ? o.detachEvent("on" + e, r) : o.removeEventListener(e, r, false);
  },
  Print: function() { window.print(); },
  Email: function(u) {
    if (!u) { u = location.href; }
    location.href = "mailto:?subject=" + ((document.title != '') ? document.title : 'Microsoft Research') + "&body=" + escape(u);
  },
  Share: function(s, u) {
    if (!u) { u = location.href; }
    u = escape(u);
    var n = "rmcshare";
    switch (s) {
      case "L":
        this.Open("/apps/c/1051.aspx?url=" + u + "&title=" + document.title, n, "");
        break;
      case "D":
        this.Open("/apps/c/1052.aspx?url=" + u + "&title=" + document.title, n, "");
        break;
      case "d":
        this.Open("/apps/c/1053.aspx?url=" + u + "&title=" + document.title, n, "");
        break;
//      case "m":
//        this.Open("http://ma.gnolia.com/bookmarklet/add?url=" + location.href + "&title=" + document.title, n, "");
//        break;
      case "T":
        this.Open("/apps/c/1054.aspx?url=" + u + "&title=" + document.title, n, "");
        break;
      case "N":
        this.Open("/apps/c/1055.aspx?url=" + u + "&title=" + document.title, n, "");
        break;
      case "F":
        this.Open("/apps/c/1056.aspx?url=" + u + "&title=" + document.title, n, "");
        break;
    }
  },
  Open: function(u, n, f) { return window.open(u, n, f); },
  NewHover: function(o, c, dx, dy, b) { this.Hovers[o] = new this.Hover(o, c, this, dx, dy, b); },
  Hover: function(o, c, r, dx, dy, b) {
    this.Clear = function() {
      clearTimeout(t);
    }
    this.Show = function(evt) {
      z.Clear();
      if (b) {
        var e = evt.target || evt.srcElement;
        var rx = evt.layerX || evt.offsetX;
        var ry = evt.layerY || evt.offsetY;
        var px = evt.pageX || (evt.clientX + document.body.scrollLeft);
        var py = evt.pageY || (evt.clientY + document.documentElement.scrollTop);
        var ow = e.clientWidth;
        var oh = e.clientHeight;
        var x = px - rx;
        var y = py + (oh - ry);
        c.style.left = x + dx + "px";
        c.style.top = y + dy + "px";
      }
      c.style.display = "block";
    }
    this.Hide = function() {
      c.style.display = "none";
    }
    this.Out = function() {
      z.Clear();
      t = setTimeout("rmc.Hovers['" + n + "'].Hide();", z.Time);
    }
    var z = this, n = o, t = null;
		this.Time = 1000;
    o = r.GE(o);
    c = r.GE(c);
    r.AE(o, "mouseover", z.Show);
    r.AE(o, "mouseout", z.Out);
    r.AE(c, "mouseover", z.Clear);
    r.AE(c, "mouseout", z.Out);
  },
  GetXml: function(p, b, cb) {
    var x;
    try {
      x = new XMLHttpRequest();
      if (b) { x.onreadystatechange = cb; }
      x.open("GET", p, b);
    }
    catch (e) {
      x = new ActiveXObject("MSXML2.DOMDocument");
      x.async = false;
    }
    return x;
  },
  AddXml: function(n, p, cb, b) {
    this.Xml[n] = this.GetXml(p, b, cb);
    try {
      this.Xml[n].send(null);
      if (!b && cb != null) { cb(); }
    }
    catch (e) {
      this.Xml[n].load(p);
      cb();
    }
  },
  AddXsl: function(n, p) {
    if (this.b.IE) {
      var x = this.GetXml(p, false);
      try {
        x.send(null);
        this.Xsl[n] = x.responseXML;
      }
      catch (e) {
        x.load(p);
        this.Xsl[n] = x;
      }
    }
    else {
      this.Xsl[n] = new XSLTProcessor();
      try {
        var w = this.GetXml(p);
        w.send(null);
        this.Xsl[n].importStylesheet(w.responseXML);
      }
      catch (e) {
        // xsl error
      }
    }
  },
  Transform: function(x, s) {
    if (this.b.IE) {
      return x.transformNode(s);
    }
    else {
      var xs = new XMLSerializer();
      return xs.serializeToString(s.transformToFragment(x, document));
    }
  },
  Calendar: function(holderId, name, cb) {
    var holder = document.getElementById(holderId);
    var month, year;
    var monthName = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
    var monthLength = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31];

    this.Show = function(selDate) {
      if (holder == null) { return; }

      var cDate = (selDate != null) ? new Date(selDate) : new Date();
      month = cDate.getMonth() + 1;
      year = cDate.getFullYear();

      var sDate = new Date(formatDate(month, 1, year));

      var mLength = monthLength[sDate.getMonth()];
      if (month == 2) { mLength = (((year % 4 == 0) && (year % 100 != 0)) || (year % 400 == 0)) ? 29 : 28; }
      var out = "<table cellspacing='0' cellpadding='0' class='cal'><tr><td class='delta prev' onclick='" + name + ".PrevMonth();'><img src='/apps/dp/i/prev.gif' alt='Previous month'/></td><td colspan='5' class='month'>" + monthName[sDate.getMonth()] + ", " + year + "</td><td class='delta next' onclick='" + name + ".NextMonth();'><img src='/apps/dp/i/next.gif' alt='Next month'/></td></tr>";
      out += "<tr><th>S</th><th>M</th><th>T</th><th>W</th><th>T</th><th>F</th><th>S</th></tr>";
      var date = 0;
      d = 1 - sDate.getDay();

      do {
        out += "<tr>";
        for (var cd = 0; cd < 7; cd++) {
          date = (d++);
          if (date > 0 && date <= mLength) { out += "<td class='day' onclick='" + name + ".Select(" + date + ");'>" + date + "</td>"; }
          else { out += "<td>&nbsp;</td>"; }
          if (date >= mLength && cd >= 6) { break; }
        }
        out += "</tr>";
      }
      while (date < mLength)

      holder.innerHTML = out + "</table>";
    };
    this.NextMonth = function() {
      this.Show(formatDate(++month, 1, year));
    };
    this.PrevMonth = function() {
      this.Show(formatDate(--month, 1, year));
    };
    this.Select = function(day) {
      cb(new Date(formatDate(month, day, year)));
    }
    var formatDate = function(m, d, y) {
      return m + "/" + d + "/" + y;
    };
  },
  Search: {
    Focus: function(o) {
      o.value = "";
      o.className = "sel";
      o = rmc.GE("goButton");
      if (o != null) { o.src = o.src.substr(0, o.src.indexOf("_"))+"_s.gif"; }
    },
    Blur: function(o) {
      if (o.value == "") { o.value = "Search Microsoft Research"; }
      o.className = "";
      o = rmc.GE("goButton");
      if (o != null) { o.src = o.src.substr(0, o.src.indexOf("_")) + "_n.gif"; }
    },
    Submit: function() {
      var q = rmc.GE("cst");
      if (q != null && q.value != "Search Microsoft Research" && q.value != "") {
        var f = rmc.GE("csf");
        if (f != null) { f.submit(); }
      }
    }
  },
  BreadCrumb: function(o) {
    var h, s = "";
    if ((h = this.GE("bcHolder")) == null) { return; }
    for (var i in o) {
      s += " > ";
      if (o[i].u != null) {
        s += "<a href='" + o[i].u + "'>" + o[i].t + "</a>";
      }
      else { s += o[i].t; }
    }
    h.innerHTML = s;
  },
  PageDepth: function() {
    if (document.documentElement) {
      var de = document.documentElement;
      var p = "http://" + location.host + "/a/bi.txt?t=2&e=0&v=" + de.clientHeight + "," + de.scrollHeight + "," + rmc.MaxS;
      rmc.AddXml("bi", p, null, false);
    }
  },
  MaxScroll: function() {
    if (document.documentElement) {
      var x = document.documentElement.scrollTop;
      if (x > rmc.MaxS) { rmc.MaxS = x; }
    }
  },
  DOE: function(s) {
    s = s.replace(/&lt;/gi, "<");
    s = s.replace(/&gt;/gi, ">");
    return s;
  },
  NewFade: function(name, holder, buttons, control) { this.Fades[name] = new this.Fade(name, holder, buttons, control); },
  Fade: function(name, holder, buttons, control) {
    var timer = null;
    holder = rmc.GE(holder);
    if (holder == null) { return; }
    buttons = rmc.GE(buttons);
    control = rmc.GE(control);
    var intervalChange = 20;
    var intervalChild = 5000;
    var amountChange = 3.5;
    var children = holder.children;
    var currentChild = 0;
    var currentPercent = 0;
    var timerAmount = intervalChild;
    var toggled = false;

    var setTimer = function() { timer = setTimeout("rmc.Fades['" + name + "'].Update();", timerAmount); }
    var nextChild = function() { return (currentChild + 1 > children.length - 1) ? 0 : currentChild + 1; }
    var setOpacity = function(o, i, f) {
      o = o.children[0];
      (rmc.b.IE && !rmc.b.V9) ? o.style.filter = "alpha(opacity=" + i + ")" : o.style.opacity = f;
      o.style.display = (i <= 0) ? "none" : "block";
    }
    var toggleButtons = function(c, n) {
      if (buttons == null) { return; }
      buttons.children[c].className = "";
      buttons.children[n].className = "sel";
    }
    var PauseMouse = function() {
      clearTimeout(timer);
      if (control != null) {
        control.children[1].style.display = "none";
        control.children[0].style.display = "block";
      }
    }
    var PlayMouse = function() {
      if (control != null) {
        control.children[0].style.display = "none";
        control.children[1].style.display = "block";
      }
      setTimer();
    }

    this.Play = function() {
      rmc.AE(holder, "mouseover", PauseMouse);
      rmc.AE(holder, "mouseout", PlayMouse);
      PlayMouse();
    }
    this.Pause = function() {
      rmc.RE(holder, "mouseover", PauseMouse);
      rmc.RE(holder, "mouseout", PlayMouse);
      PauseMouse();
    }
    this.Update = function() {
      if (currentPercent == 0) { timerAmount = intervalChange; }
      else if (currentPercent > 100) {
        timerAmount = intervalChild;
        currentChild = nextChild();
        currentPercent = 0;
        setTimer();
        toggled = false;
        return;
      }
      currentPercent += amountChange;
      if (!toggled && currentPercent > 5) { toggleButtons(currentChild, nextChild()); toggled = true; }
      setOpacity(children[nextChild()], currentPercent, (currentPercent / 100));
      setOpacity(children[currentChild], (100 - currentPercent), 1 - (currentPercent / 100));
      setTimer();
    }
    this.GoTo = function(evt) {
      var n;
      for (n = 0; n < buttons.children.length; n++) {
        var e = evt.target || evt.srcElement;
        if (e === buttons.children[n]) { break; }
      }
      clearTimeout(timer);
      setOpacity(children[nextChild()], 0, 0);
      setOpacity(children[currentChild], 0, 0);
      setOpacity(children[n], 100, 1);
      toggleButtons(currentChild, n);
      currentChild = n;
      timerAmout = intervalChild;
      setTimer();
    }
    var z = this;
    if (buttons != null && holder.children.length > 1) {
      for (var x = 0; x < holder.children.length; x++) {
        var d = document.createElement("div");
        if (x == 0) { d.className = "sel"; }
        rmc.AE(d, "click", z.GoTo);
        buttons.appendChild(d);
      }
    }
    if (control != null) {
      rmc.AE(control.children[0], "click", z.Play);
      rmc.AE(control.children[1], "click", z.Pause);
    }
  }
};

    </SCRIPT>
     
<SCRIPT language="javascript" type="text/javascript">
        function OpenFeedback() {
            var cci = rmc.GE("clickCountImg");
            if (cci != null) { cci.src = "/c/1171"; }
            rmc.Open("/apps/feedback/Feedback.aspx", "popwindow", "width=500px,height=540px,status=0,directories=0");
        }
    </SCRIPT>
		   
<META name="description" content="Similarity"> 
<META name="GENERATOR" content="MSHTML 11.00.9600.18450"></HEAD>
<BODY>	 <!--NOINDEX_START-->    		 <!--<div id="cShare" class="pop dn">
			<div class="h">Share this page</div>
			<ul>
				<li><a href="javascript:rmc.Share('L');void(0);">Live Favorites</a></li>
				<li><a href="javascript:rmc.Share('D');void(0);">Digg</a></li>
				<li><a href="javascript:rmc.Share('d');void(0);">del.icio.us</a></li>
				<li><a href="javascript:rmc.Share('T');void(0);">Twitter</a></li>
				<li><a href="javascript:rmc.Share('N');void(0);">Newsvine</a></li>
				<li><a href="javascript:rmc.Share('F');void(0);">Facebook</a></li>
			</ul>
		</div>-->			 
<DIV><A name="rmcTop"></A>			 
<DIV class="center sw pr" id="chTB"><!-- <div id="chLogo"><a href="/c/1040" onClick="stc(this, 1)"><img alt="Microsoft Research" src="/a/i/c/logo_msr.png"/></a></div>-->
			   <!--div id="chLogo"><a href="/c/1040" onClick="stc(this, 2)"><img alt="Microsoft Research" src="/a/i/c/logo_msr.png"/></a></div-->
				 <!--<div id="chSearch">
					<form method="get" id="csf" onsubmit="rmc.Search.Submit();return false;" action="/apps/dp/search.aspx"/>
						<input class="pa" onfocus="rmc.Search.Focus(this);" onblur="rmc.Search.Blur(this);" name="q" id="cst" type="text" value="Search Microsoft Research" />
						<input class="pa" alt="Submit search" id="goButton" type="image" src="/a/i/c/search_n.gif"/>
				    </form>
				</div>-->								     
<DIV id="chTer"><!-- <a href="/c/1048" onClick="stc(this, 3)">
						    <b class="item t5 fl">
							    <div>Videos</div> 
						    </b>
					    </a>-->					     <!--<a href="/c/1042" onClick="stc(this, 4)">
						    <b class="item t4 fl">
							    <div>Projects</div>
						    </b>
					    </a>-->					     <!--<a href="/c/1043" onClick="stc(this, 5)">
						    <b class="item t2 fl">
							    <div>Publications</div>
						    </b>
					    </a>-->					     <!-- <a href="/c/1044" onClick="stc(this, 6)">
						    <b class="item t3 fl">
							   <div>People</div>
						    </b>
					    </a>-->					     <!--<a href="/c/1045" onClick="stc(this, 7)">
						    <b class="item t1 fl">
							    <div>Downloads</div>
						    </b>
					    </a>-->				     </DIV></DIV>
<DIV class="center sw" id="shadow"><!--<div id="top">
					<img src="/a/i/c/s_top.png"/>
					<img src="/a/i/c/s_top.png" /
				</div>-->				 
<DIV id="border">
<DIV id="chNav"><!--<div id="chP">
               <table cellspacing="0" cellpadding="0" border="0">
                <col width="6"/>
                <tr>
                  <td>&nbsp;</td>
      		           <div id="ctl00_ctl00_Navigation2_holder"><td>
  <div><a href="/c/1000" onClick="stc(this, 8)">Home</a></div>
</td>
<td class="sel">
  <div><a href="/c/1010" onClick="stc(this, 9)">Our Research</a></div>
</td>
<td>
  <div><a href="/c/1020" onClick="stc(this, 10)">Connections</a></div>
</td>
<td>
  <div><a href="/c/1030" onClick="stc(this, 11)">Careers</a></div>
</td>
<td>
  <div><a href="/c/1180" onClick="stc(this, 12)">Hub</a></div>
</td></div>

                  <td width="100%">&nbsp;</td>
                </tr>
              </table>		
      		  </div>-->	      		<!--  <div id="chS">
			  <div id="ctl00_ctl00_Navigation1_holder">
			  <ul class="horiz">
  
  <li class="first"><a href="/c/1011" onClick="stc(this, 13)">Worldwide Labs</a></li>
  <li class=""><a href="/c/1012" onClick="stc(this, 14)">Research Areas</a></li>
  <li class="last"><a href="/c/1013" onClick="stc(this, 15)">Research Groups</a></li>
  </ul>
</div>
</div>--> <!--      		  <div id="chPM"><div id="ctl00_ctl00_ctl00_holder"><table cellpadding="0" cellspacing="0" border="0" id="pmleft"><tr><td valign="top"><a href="/c/1204" onClick="stc(this, 16)"><img border="0" src="/en-us/images/ads/chrome/featured_videos_chrome_ad_3.png" alt="Featured Videos from Microsoft Research" title="Featured Videos from Microsoft Research"></a></td></tr></table></div>
</div>
    		  </div>
					<div id="crumbBar">
						<div id="tools">
	<ul class="horiz">
	    <li>
	        <a href="javascript:rmc.Share('T');void(0);"><img title="Share this page on Twitter" alt="Share this page on Twitter" src="/a/i/c/twitter_16x16.png" border="0" width="16" height="16" /></a>
	        <a href="javascript:rmc.Share('F');void(0);"><img title="Share this page on Facebook" alt="Share this page on Facebook " src="/a/i/c/facebook_16x16.png" border="0" width="16" height="16" /></a>
	        <a href="javascript:rmc.Share('D');void(0);"><img title="Share this page on Digg" alt="Share this page on Digg" src="/a/i/c/digg_16x16.png" border="0" width="16" height="16" /></a>
	        <a href="javascript:rmc.Share('d');void(0);"><img title="Share this page on Del.icio.us" alt="Share this page on Del.icio.us" src="/a/i/c/delicious_16x16.gif" border="0" width="16" height="16" /></a>
	        <a href="/c/1057" onClick="stc(this, 17)"><img title="Read the Inside Microsoft Research blog" alt="Read the Inside Microsoft Research blog" src="/a/i/c/blog_16x16.png" border="0" width="16" height="16" /></a>
	    </li>
	    <li>
	        <a href="javascript:rmc.Email();void(0);"><img title="E-mail this page" alt="E-mail this page" src="/a/i/c/t_email.gif" border="0" width="16" height="16" /></a>
	        <a href="javascript:rmc.Print();void(0);"><img title="Print this page" alt="Print this page" src="/a/i/c/t_print.gif" border="0" width="16" height="16" /></a>
	    </li>
	    <li class="last">
	        <a href="/c/1046" onClick="stc(this, 18)"><img title="RSS feeds" alt="RSS feeds" src="/a/i/c/rss.gif" border="0" width="18" height="18" /></a>
	    </li>
	</ul>
</div>-->						 <!--<a href="/c/1047" onClick="stc(this, 19)"><img alt="Home" border="0" src="/a/i/c/bc_home.png" /></a>
						<span id="bcHolder">
		&gt; Projects
		&gt; Similarity</span>-->					 </DIV><!--NOINDEX_STOP-->					 
<DIV id="contentArea">
<DIV class="zone" id="mainZone">
<DIV class="compositeModule_1Zone ">
<DIV class="zone">
<DIV class="title deM"><B>Concept based Short Text Stream Classification with Topic Drifting Detection</B>
<DIV class="cl"></DIV></DIV>
<DIV class="conM ">
<P>&nbsp;</P><!--<P align=center><SPAN style="MARGIN: 0px; WIDTH: 230px" id=c97b486e-e8f8-438b-adde-6bf9a444a7c5 class="ImageBlock fn"><IMG id=Imagec97b486e-e8f8-438b-adde-6bf9a444a7c5 src="/en-us/projects/probase/probaselogo.gif"><SPAN id=ImageCaptionc97b486e-e8f8-438b-adde-6bf9a444a7c5 class="ImageCaptionCoreCss ImageCaption"></SPAN></SPAN></P>
<TABLE cellSpacing=0 cellPadding=0 width="100%">
<TBODY>
<TR>
<TD align=center>
<P align=center>Overview |&nbsp;<A href="/en-us/projects/probase/statistics.aspx" target=_self onClick="stc(this, 21)">Data Statistics</A>&nbsp;| <A href="/en-us/projects/probase/applications.aspx" target=_self onClick="stc(this, 22)">Applications</A>&nbsp;|&nbsp;<A href="/en-us/projects/probase/release.aspx" target=_self onClick="stc(this, 23)">Release</A>&nbsp;| <A href="/en-us/projects/probase/publications.aspx" target=_self onClick="stc(this, 24)">Documents and Publications</A></P></TD></TR>
<TR>
<TD ALIGN="center" >
<P>&nbsp;</P>
<P>&nbsp;</P></TD></TR></TBODY></TABLE>
--> 
<P>Short text stream classification is a very challenging
and significant task due to the characteristics of short
length, weak signal, high velocity and especial topic drift
in short text stream. However, this challenge has received
little attention from the research community. Motivated by
this, we propose a new feature extension approach for short
text stream classification using a large scale, general purpose
semantic network obtained from a web corpus. Our approach
is built on an incremental ensemble classification model. First,
in terms of the open semantic network, we introduce more
semantic contexts in short texts to make up of the data sparsity.
Meanwhile, we disambiguate terms by their semantics to
reduce the noisy impact. Second, to effectively track the hidden
topic drifts, we propose a concept cluster based topic drifting
detection method. Finally, extensive experiments demonstrate
our approach can detect topic drifts effectively compared to
several well-known concept drifting detection methods in data
stream. Meanwhile, our approach can perform best in the
classification of text data stream compared to several stateof-
the-art short text classification approaches.</P><!--<P><SPAN style="MARGIN: 0px; WIDTH: 28px" id=dc5dbdce-0a30-4c97-8cec-a9b1678f5d98 class="ImageBlock fn"><IMG style="WIDTH: 28px" id=Imagedc5dbdce-0a30-4c97-8cec-a9b1678f5d98 src="/en-us/projects/probase/new.gif"><SPAN id=ImageCaptiondc5dbdce-0a30-4c97-8cec-a9b1678f5d98 class="ImageCaptionCoreCss ImageCaption"></SPAN></SPAN>We are pleased to announce the release of Probase v0.10. You can find more release information <A href="/en-us/projects/probase/release.aspx" target=_new onClick="stc(this, 25)">here</A> (only available for internal use for now).</P>
--> 
<H2>Introduction</H2>
<P>Short texts are prevalent on the Web, such as search
snippets and tweets. Unlike traditional normal texts such as
news articles, short texts refer to the length of the shorter
text form. For example, a tweet has a 140 character limit.
In recent years, these short texts swept the world at an
alarming rate, and have produced a large quantity of data
stream. We call them as short text streams. However, short
text stream classification is a very challenging task, owing
to the fact that these data have inherent defects such as short
length, weak signal and high ambiguity for each short text,
meanwhile, because of the explosive growth and popularity
of short textual content.</P>
<P>Given the characteristics of these short text streams, there
are several challenges with applying the traditional text
classification [1] to build models. This is because first, each
short text does not contain enough statistical signals to make
the analysis meaningful. Second, the limited contexts make
it more difficult to identify the senses of ambiguous words in
each short text. Third, they present the characteristics of data
streams as being continuous, high-volume, open-ended and
topic drifting in short texts. Meanwhile, existing short text classification approaches rarely focus on the characteristics
of data stream. It is hence a challenge for them in the
tackling of short text stream classification. To handle of the
short text classification, existing approaches mainly follow
two directions to enrich the short text. The first one is to
extend the feature space only using the rules or statistical
information hidden in the current short text contexts [2],
called the self-resource based approach. While the other is
to extend the feature space by external sources, called the
external resource based approach, and it can be divided into
four categories[3], [4], including link based approach [5],
Web search based approach [6], taxonomy based approach
[7] and topic based approach [8].</P>
<H2>Our Approach</H2>
<P>However, all of the aforementioned approaches are batch
algorithms, they are hence not suitable for short text stream
classification especially in the cases with topic drifts. Thus,
we propose a new feature extension approach for short text
stream classification using a large scale, general purpose
semantic network obtained from a web corpus. Our contributions
are as follows.</P>
<P>The main contributions of this paper are:</P>
<P>First, our approach produces higher
classification accuracy. We use an open semantic network
called Probase1 instead of other popular taxonomy knowledgebases
(such as Wikipedia) as the external resources. In
terms of the taxonomy in Probase, our approach introduces
more semantic contexts hidden in short texts to make up
of the data sparsity. Meanwhile, our approach seeks to
disambiguate terms in short texts and thus excludes noises
from irrelevant senses of terms. It is conducive to improve
the classification accuracy.</P>
<P>Second, our approach can detect
the topic drifts effectively. Contrary to the classificationerror
based concept drifting method, we use the concept
clusters of terms to represent the data distributions of each
chunk, and then compute the distance between concept
clusters to detect the topic drifts hidden in short text streams.</P>
<H2>Data Set </H2>
<P><A herf= "http://jwebpro.sourceforge.net/data-web-snippets.tar.gz" >Web Search Snippets</A>: Search snippets consists of three
parts: a URL, a short title and a short text description. The
search snippets were selected from the results of web search
transaction using predefined phrases of different domains.
There are eight categories with 12340 records.</P>
<P><A herf= "http://acube.di.unipi.it/tmn-dataset/" >News</A>:News is a dataset of 32K english news extracted from RSS
feeds of popular newspaper websites. It has seven categories.
Each news in the file has the structure of title, description
and category. We only extract titles as the data set here.</P>
<!--
<P>It turns out what we need in order to act like a human in the above two examples is nothing more than knowledge about concepts (e.g., persons and animals) and the ability to conceptualize (e.g., cats are animals). This is not a coincidence. Psychologist Gregory Murphy began his highly acclaimed book with the statement 揅oncepts are the glue that holds our mental world together&#65533;. Nature magazine book review pointed out 揥ithout concepts, there would be no mental world in the first place&#65533;. Doubtless to say, having concepts and the ability to conceptualize is one of the defining characteristics of humanity. The question is then: How do we pass human concepts to machines, and how do we enable machines to conceptualize?</P>
<P>Knowledge in Probase is harnessed from billions of web pages and years worth of search logs -- these are nothing more than the digitized footprints of human communication. In other words, Probase uses the world as its model.</P>
<P align=center><SPAN style="MARGIN: 0px; WIDTH: 481px" id=05913a85-cd95-4d8b-afa6-18011f34954f class="ImageBlock fn"><IMG style="WIDTH: 481px" id=Image05913a85-cd95-4d8b-afa6-18011f34954f src="/en-us/projects/probase/probasenew2.jpg"><SPAN id=ImageCaption05913a85-cd95-4d8b-afa6-18011f34954f class="ImageCaptionCoreCss ImageCaption"></SPAN></SPAN></P>
<P align=center><B>Figure 1: A snippet of Probase's core taxonomy</B></P>
<P><B>Figure 1</B> shows what is inside&nbsp;Probase. The knowledgebase consists of <B><I>concepts</B></I> (e.g. emerging markets), <B><I>instances</B></I> (e.g., China), <B><I>attributes</B></I> and <B><I>values</B></I> (e.g., China's population is 1.3 billion), and <B><I>relationships</B></I> (e.g., emerging markets, as a concept, is closely related to newly industrialized countries), all of which are automatically derived in an unsupervised manner.</P>
<P>But Probase is much more than a traditional ontology/taxonomy.&nbsp; Probase is unique in two aspects. First, <B>Probase has an extremely large concept/category space (2.7 million categories).</B> As these concepts are automatically acquired from web pages authored by millions of users, it is probably true that they cover most concepts in our mental world (about worldly facts). Second, <B>data in Probase, as knowledge in our mind, is not black or white.</B> <STRONG>Probase quantifies the uncertainty.</STRONG> These serve as the priors and likelihoods that become the foundations of probabilistic reasoning in Probase. </P>
<P>Our mental world contains many concepts about worldly facts, and Probase tries to duplicate them. The core taxonomy of Probase alone contains above 2.7 million concepts. Figure 2 shows their distribution. The Y axis is the number of instances each concept contains(logarithmic scale), and on the X axis are the 2.7 million concepts ordered by their size. In contrast, existing knowledge bases have far fewer concepts (Freebase [3] contains no more than 2,000 concepts, and Cyc [7] has about 120,000 concepts), which fall short of modeling our mental world. As we can see in Figure 2, besides popular concepts such as 揷ities&#65533; and 搈usicians&#65533;, which are included by almost every general purpose taxonomy, Probase has millions of long tail concepts such as 揳nti-parkinson treatments&#65533;, "celebrity wedding dress designers&#65533; and 揵asic watercolor techniques&#65533;, which cannot be found in Freebase or Cyc. Besides concepts, Probase also has a large data space (each concept contains a set of instances or sub-concepts), a large attribute space (each concept is described by a set of attributes), and a large relationship space (e.g.,搇ocatedIn&#65533;, "friendOf&#65533;, "mayorOf&#65533;, as well as relationships that are not easily named, such as the relationship between apple and Newton.)</P>
<P><B align="center"><SPAN style="MARGIN: 0px; WIDTH: 900px" id=f2424153-3b26-42e7-a9d7-820372e15852 class="ImageBlock fn"><IMG style="WIDTH: 900px; HEIGHT: 357px" id=Imagef2424153-3b26-42e7-a9d7-820372e15852 src="/en-us/projects/probase/conceptcurves2_3.png"><SPAN id=ImageCaptionf2424153-3b26-42e7-a9d7-820372e15852 class="ImageCaptionCoreCss ImageCaption"></SPAN></SPAN></P></B>
<P align=center><B>Figure 2: Frequency distribution of the 2.7 million concepts</B></P>
--> 
<H2>Experiment Results</H2>
<P>Table 1 shows the benchmark data sets used in our experiments. 
<!--Due to the space limit, other experimental results are not shown here, you can get details from Download.-->
</P>
<P align="center"><B>Table 1: DATA SETS USED IN THE EXPERIMENTS</B></P>
<P>
<TABLE width="700" align="center" class=" borderColumns borderRows tableBorder" 
cellSpacing="0" cellPadding="0">
  <TBODY>
  <TR>
    <TD align="center"><B>domain</B></TD>
    <TD align="center"><B>#documents</B></TD>
    <TD align="center"><B>domain</B></TD>
    <TD align="center"><B>#documents</B></TD>
    </TR>
  <TR>
    <TD align="center" colspan="2">Web Search Snippets</TD>
    <TD align="center"colspan="2">News</TD>
</TD>
</TR>
<TR>
    <TD align="center">Business</TD>
    <TD align="center">1500</TD>
    <TD align="center">Sport</TD>
    <TD align="center">8190</TD>
</TR>
<TR>
    <TD align="center">Computer</TD>
    <TD align="center">1500</TD>
    <TD align="center">Business</TD>
    <TD align="center">5367</TD>
</TR>
<TR>
    <TD align="center">Culture-Arts-Ent</TD>
    <TD align="center">2210</TD>
    <TD align="center">U.S.</TD>
    <TD align="center">4783</TD>
</TR>
<TR>
    <TD align="center">Education-Science</TD>
    <TD align="center">2660</TD>
    <TD align="center">Health</TD>
    <TD align="center">1851</TD>
</TR>
<TR>
    <TD align="center">Engineering</TD>
    <TD align="center">370</TD>
    <TD align="center">Sci&amp;Tech</TD>
    <TD align="center">2872</TD>
</TR>
<TR>
    <TD align="center">Politics-Scienty</TD>
    <TD align="center">1500</TD>
    <TD align="center">Entertainment</TD>
    <TD align="center">3286</TD>
</TR>
<TR>
    <TD align="center">Health</TD>
    <TD align="center">1180</TD>
    <TD align="center">World</TD>
    <TD align="center">6255</TD>
</TR>
<TR>
    <TD align="center">Sport</TD>
    <TD align="center">1420</TD>
    <TD align="center">/</TD>
    <TD align="center">/</TD>
</TR>
<TR>
    <TD align="center">total</TD>
    <TD align="center">12340</TD>
    <TD align="center">total</TD>
    <TD align="center">32604</TD>
</TR>
  </TBODY></TABLE>
<P></P>
<!--<H2>Download: Complete Data Set</H2>--> <!--
<P>We make a bold claim that Probase is a knowledgebase about concepts in our mental world because the concepts in Probase are harnessed from billions of web pages authored by millions of people (see Section 3). With such a rich concept space, Probase has much better chance to understand text in natural language (see Section 4). Indeed, we studied 2 years&#65533; worth of Microsoft抯 Bing search log, and found that 85% of the searches contain concepts and/or instances that exist in Probase. It means Probase can be a powerful tool to interpret user intention behind search.</P>
<P>Another feature of Probase is that it is probabilistic, which means every claim in Probase is associated with some probabilities that model the claim抯 correctness, typicality, ambiguity, and other characteristics. The probabilities are derived from evidences found in web data, search log data, and other existing taxonomies. For example, for typicality (between concepts and instances), Probase contains the following probabilities:</P>
<UL>
<LI>P(C=company|I=apple): How likely people will think of the concept 揷ompany&#65533; when they see the word 揳pple&#65533;. </LI>
<LI>P(I=steve jobs|C=ceo): How likely 搒teve jobs&#65533; will come into mind when people think about the concept 揷eo&#65533;.</LI></UL>
<P>Probase also has typicality scores for concepts and attributes. Another important score in Probase is the similarity between any<BR>two concepts y1 and y2 (e.g., <EM>celebrity</EM> and <EM>famous politicians</EM>). Thus Probase can tell that <EM>natural disasters</EM> and <EM>politicians</EM> are very different concepts, <EM>endangered species</EM> and <EM>tropical rainforest plants</EM> have certain relationships, while <EM>countries</EM> and <EM>nations</EM> are almost the same concepts.</P>
<P>These probabilities serve as priors and likelihoods for Bayesian reasoning on top of Probase. In addition, the probabilistic nature of Probase also enables it to incorporate data of varied quality from heterogeneous sources. Probase regards external data as evthese probabilities serve as priors and likelihoods for Bayesian reasoning on top of Probase. </P></div>
        <div style="clear:both;"></div>
        <div class="conM "><H2>Applications</H2>
<P>The goal of our semantic similarity measurement approach is to accuratly compute the semantic similarity between terms. to enable machines to better understand human communication. For example, in natural language processing and speech analysis, knowledgebases can help reduce the ambiguities in language. As Probase has a knowledgebase as large as the concept space (of wordly facts) in a human mind, it has unique advantages in these applications.</P>
<P>Besides, with the probabilistic knowledge provided by Probase, we build several interesting applications, such as topic search, web table search and document&nbsp;understanding,&nbsp;shown in Figure 3.</P>
<P align=center><SPAN style="MARGIN: 0px; WIDTH: 850px" id=186f2c32-3da1-49e5-8ab6-562eeb443c3a class="ImageBlock fn"><IMG style="WIDTH: 850px; HEIGHT: 484px" id=Image186f2c32-3da1-49e5-8ab6-562eeb443c3a src="/en-us/projects/probase/probase_overview.png"><SPAN id=ImageCaption186f2c32-3da1-49e5-8ab6-562eeb443c3a class="ImageCaptionCoreCss ImageCaption"></SPAN></SPAN><BR><B>Figure 3: Overview of&nbsp;Probase and Its Applications</B></P></div>
-->         
<DIV style="clear: both;"></DIV>
<DIV class="conM ">
<H2>Used Data Sets: Download</H2>
<P>More Details Refer to <A onclick="stc(this, 26)" href="http://121.42.218.45/peipeili/Used-Data-Sets-and-demo.rar" 
target="_new"> Used Data Sets</A>.</P></DIV>
<DIV style="clear: both;"></DIV>
<DIV class="conM ">
<H2>Source codes: Download</H2>
<P>More Details Refer to <A onclick="stc(this, 26)" href="http://121.42.218.45/peipeili/ShortTextClassification-src.rar" 
target="_new"> Source codes</A>.</P></DIV>
<DIV style="clear: both;"></DIV>
<DIV class="conM ">
<H2>References</H2>
<P>[1] K. Nigam, A. McCallum, S. Thrun, and T. Mitchell, “Text
classification from labeled and unlabeled documents using
em,” Machine learning, vol. 39, no. 2, pp. 103–134, 2000.</P>
<P>[2] X. Cheng, X. Yan, Y. Lan, and J. Guo, “Btm: Topic modeling
over short texts,” IEEE Transactions on Knowledge and Data
Engineering, vol. 26, pp. 2928–2941, 2014.</P>
<P>[3] M. Chen, X. Jin, and D. Shen, “Short text classification improved
by learning multi-granularity topics,” in Proceedings
of IJCAI’11, 2011, pp. 1776–1781.</P>
<P>[4] L. Gao, S. Zhou, and J. Guan, “Effectively classifying short
texts by structured sparse representation with dictionary filtering,”
Information Sciences, vol. 323, pp. 130–142, 2015.</P>
<P>[5] X. Wang, Y. Wang, W. Zuo, and G. Cai, “Exploring social
context for topic identification in short and noisy texts,” in
AAAI’15, 2015, pp. 1868–1874.</P>
<P>[6] D. Bollegala, Y. Matsuo, and M. Ishizuka, “A web search
engine-based approach to measure semantic similarity between
words,” IEEE TKDE, vol. 23, pp. 977–990, 2011.</P>
<P>[7] M. SHIRAKAWA, K. NAKAYAMA, T. HARA, and
S. NISHIO, “Wikipedia-based semantic similarity measurements
for noisy short texts using extended naive bayes,” IEEE
Transactions on Emerging Topics in Computing, vol. 3, pp.
205–219, 2015.</P>
<P>[8] X. Phan, C. Nguyen, D. Le, L. Nguyen, S. Horiguchi, and
Q. Ha, “A hidden topic-based framework toward building
applications with short web documents,” IEEE Transactions
on Knowledge and Data Engineering, vol. 23, pp. 961–976,
2011.</P>
</DIV>
<DIV class="conM ">
<H2>Contact</H2>
<P><A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://ci.hfut.edu.cn/index/teacherinfo/tid/522" 
target="_new" alt="">Peipei Li</A> (peipeili@hfut.edu.cn): Hefei University of Technology<BR>
<A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://haixun.olidu.com/" 
target="_new" alt="">Lu He</A> (luhe@mail.hfut.edu.cn): Hefei University of Technology <BR><A title="" style="zoom: 1;" onclick="stc(this, 29)" 
target="_new" alt="">Xuegang Hu</A> (jsjxhuxg@hfut.edu.cn): Hefei University of Technology<BR>
<A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://ci.hfut.edu.cn/index/teacherinfo/tid/477" 
target="_new" alt="">Yuhong Zhang</A> (zhangyuhong@hfut.edu.cn): Hefei University of Technology<BR>
<A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://ci.hfut.edu.cn/index/teacherinfo/tid/521" 
target="_new" alt="">Lei Li</A> (lilei@hfut.edu.cn): Hefei University of Technology<BR>
<A title="" style="zoom: 1;" onclick="stc(this, 30)" href="http://www.ucs.louisiana.edu/~xxw8007/" 
target="_new" alt="">Xindong Wu</A> (xwu@uvm.edu): University of Louisiana</P>
<P class="smallText"></P>
<P class="smallText">&nbsp;</P></DIV>
<DIV style="clear: both;"></DIV></DIV>
<DIV style="clear: left;"></DIV></DIV></DIV></DIV><!--NOINDEX_START-->					 
<DIV class="cl"></DIV>
<DIV class="bt" id="bGrad"></DIV></DIV></DIV><!--<div id="ctl00_ctl00_ctl01_holder" class="shellFooter"><div id="footer" class="center sw"><div class="fr"><span>&copy;2012 Microsoft Corporation. All rights reserved.</span><a href="/c/1064" onClick="stc(this, 31)"><img alt="Microsoft" title="Microsoft" src="/a/i/c/logo_ms.png" border="0"></a></div><ul class="horiz"><li class="first"><a href="/c/1060" onClick="stc(this, 32)">Contact</a></li><li class=""><a href="/c/1061" onClick="stc(this, 33)">Terms</a></li><li class=""><a href="/c/1062" onClick="stc(this, 34)">Trademarks</a></li><li class=""><a href="/c/1063" onClick="stc(this, 35)">Privacy and Cookies</a></li><li class=""><a href="/c/1065" onClick="stc(this, 36)">Code of Conduct</a></li><li class="last"><a href="javascript:OpenFeedback();">Feedback</a></li></ul></div></div>
			-->			 
<SCRIPT type="text/javascript">
				rmc.AE(window, "unload", rmc.PageDepth);
				rmc.AE(window, "scroll", rmc.MaxScroll);
			</SCRIPT>
		 </DIV><!--NOINDEX_STOP-->         <!-- this used to click count when feedback popup is clicked --> 
        <IMG id="clickCountImg" style="display: none;">	 
<SCRIPT type="text/javascript">
function stc(e,linkIndex){if(document.images){var linkText;if(navigator.appName.toLowerCase()=="microsoft internet explorer"){linkText=e.innerText}else{linkText=e.textContent}if(linkText==""){if(e.firstChild){var firstChild=e.firstChild.nodeName.toUpperCase();if(firstChild=="IMG"){linkText="Image: "+getName(e.firstChild.getAttribute('src'))}}else{var nodeName=e.nodeName.toUpperCase();if(nodeName=="AREA"){linkText="ImageMap: "+e.href}}}if(linkText==""){linkText=e.href}(new Image()).src="/a/i/stg.gif?f="+escape(document.location.href)+"&t="+escape(e.href)+"&i="+linkIndex+"&n="+escape(trimString(linkText))}}function getName(s){if(s.lastIndexOf('/')>=0){return(s.substring(s.lastIndexOf('/')+1,s.length))}else{return(s)}}function trimString(s){return(s.replace(/^\s*/,"").replace(/\s*$/,""))}
</SCRIPT>
 </DIV></BODY></HTML>


All benchmark data sets are used in our experiments below. 
Web search Snippets: http://jwebpro.sourceforge.net/data-web-snippets.tar.gz
News: http://acube.di.unipi.it/tmn-dataset/

How to use our source codes?
1. The solution is built on Visual Studio 2010 C# plateform.
2. The main function is in the project of LibSVMSharp.Examples.Classification
Train using SVM classifier and implement the concept drifting detection, namely the function of TrainAndDriftDetectAndTest is called in the main function.
All parameter settings are below. （You can use the default values in the parameter settings).
 /// <summary>
 /// Training by SVMClassifier over data chunks and concept drfiting detection
        /// </summary>
        /// <param name="thresOfWin">thresOfWin: the threshold of the size of window (data chunk), default: 0.5</param>
        /// <param name="parameter">parameter: the parameters of SVM training</param>
        /// <param name="modelMaxNum">modelMaxNum: the size limit of ensembling models</param>
        /// <param name="thresOfWin">thresOfWin: the threshold of window</param>
        /// <param name="slidWinSize">sildWinSize: the size of the sliding window,default: 2000</param>
        /// <param name="maxW">maxW: the maximum size of the sliding window, default: 1000</param>
        /// <param name="minW">minW: the minmum size of the sliding window, default: 200</param>
        /// <param name="srcTextOfAllTerms">srcTextOfAllTerms: the directory of reading all terms including the dominant clusters for entities</param>
        /// <param name="srcTextOfDC">srcTextOfDC: the directory of reading the dominant clusters for entities</param>
        /// <param name="srcTextOfVSM">srcTextOfVSM: the directory of reading the feature space for classifier generation, the file can be "CVSM" or "WCVSM"</param>
        /// <param name="chunkSize">chunkSize: the chunk size in the concept drifting detecton</param>
        /// <param name="labelPos">labelPos: the postition of labels, default: 0 (at the begining) </param>
        /// <param name="basicAlg">basicAlg: the basic algorithm, default: "SVM" </param>
        /// <param name="fadingFactor">fadingFactor: the value of fading factor, eg., 0.995</param>
        /// <param name="estimatorType">estimatorType: prequential error estimator in sliding window/uing fading factor</param>
        /// <param name="serverName">serverName: the server name, default: "LPP-PC" </param>
        /// <param name="dataSrc">dataSrc: the database name, default: "corev52" </param>
        /// <param name="bUseSynonym">bUseSynonym: whether it uses the synonym data or not, default value: false </param>
        /// <returns></returns>
		
3. in the folder of demo, we give an example to show how to run our executable file.
the batch file:  F:\shortTextData\News\train+test\title\allData titleAll.ReOrgConcept200.termRecog-tfidf.VSMWithCluster titleAll.ReOrgConcept200.termRecog-tfidf.dominantCluster titleAll.ReOrgConcept200.termRecog-tfidf.SVSM 50 0 false 0.75 cosine KNN 1000 0.85 prequentialByFading 0

In order to run this batch file, you need the following prepared data:
(1) titleAll.ReOrgConcept200.termRecog-tfidf.VSMWithCluster 
(2) titleAll.ReOrgConcept200.termRecog-tfidf.dominantCluster
(3) titleAll.ReOrgConcept200.termRecog-tfidf.SVSM
These data can be obtained by the funtions in the project of "ConceptualizationTerms"
a) step 1: term recognition, namely call the funtion RecognizeTerms() in the main function;
b) step 2: generate vector space model for texts with term recognition, namely call the funtion GenVSM() in the main function;
b) step 3: Disambiguation, namely call the funtion DisambiguateTerms() in the main function; 
More details refer to examples in the main function  of "ConceptualizationTerms" project.

In this batch file, description of input parameters is below:
string directory = args[0]; //the path directory: F:\shortTextData\News\train+test\title\allData
string srcTextOfAllTerms = args[1]; // source data with term recognition
string srcTextOfDC = args[2]; // source data with dominant senses
string srcTextOfVSM = args[3]; //source data with vectorization using senses
int chunkSize = Convert.ToInt32(args[4]);//data chunk, default '200'; 
int labelPos = Convert.ToInt32(args[5]);//the label position given the training data, default: at the beginig, namely '0';
bool labelUnKnown = Convert.ToBoolean(args[6]);//whether the label is known or not, defualt: known, namely 'false', if unknown, use 'true' 
double thresInitCenter = Convert.ToDouble(args[7]);//the threshold used in the concept cluster based topic drifting detection, default: '0.5'
string distEvalType = args[8];//the similarity function, default: cosine
string basicAlg = args[9];//the prediction function, default: "KNN"
Int64 slidWinSize = Convert.ToInt64(args[10]);//the window size
double drifThres = Convert.ToDouble(args[11]);//the threshold used in the topic drifting detection, if the distance between clusters is larger than this threshold, drift is considered.
string estimatorType = args[12]; //the type of topic drifting detection, using prequential prediction by sliding window or by fading factor
double fadingFactor = 0;
if (estimatorType == "prequentialByFading")//in the topic drifting detection, if you select the prequential test by fading factor, it is necessary to set the value of fading factor.
    fadingFactor = Convert.ToDouble(args[13]);

