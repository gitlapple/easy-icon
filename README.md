<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Easy-ICON - 一个简单易用的icon字体库</title>
    <meta name="keywords" content="字体图标库,js字体图标库,web图标">
    <meta name="description" content="Easy-ICON - 一个简单易用的icon字体库">
    <link rel="stylesheet" href="./dist/easy-icon.min.css">
    <link rel="stylesheet" href="./assets/index.css">
    <link rel="stylesheet" href="./assets/navi.css">
    <link rel="stylesheet" href="./assets/doc.css">
    <script src="./assets/index.js"></script>
    <script src="./assets/navi.js"></script>
</head>

<body>
    <div id='navi'>
        <div id='logo'>
            <a class='link-item' href='https://github.com/theajack/easy-icon' target="blank"><img src="./assets/images/logo.png" alt=""></a>
        </div>
        <div class='navi-w'>
            <span class='navi-item active' navi-target='iconShow'>图标</span>
            <span class='navi-item' navi-target='useBlock'>使用</span>
            <span class='navi-item' navi-target='spinBlock'>旋转</span>
            <span class='navi-item' navi-target='sizeBlock'>尺寸</span>
        </div>
        <div class='link-w'>
            <a class='link-item' href='https://www.theajack.com/easy-icon' target="blank">EN</a>
            <a class='link-item' href='https://github.com/theajack/easy-icon' target="blank"><i class="ei-github"></i></a>
        </div>
    </div>
    <div id="iconsExample" class="text">
        <div id="iconShow" class="t-center">
            <span id='icons'>
                <i class="ei-resize"></i>
                <i class="ei-resize icon-middle"></i>
                <i class="ei-resize icon-large"></i>
                <i class="ei-resize icon-slarge"></i>
            </span>
            <div class='input-w'>
                <input type="text" id='fullHtmlInput' readonly="" class="ei-input">
                <button class="ei-btn code-copy" title="复制" onclick="copyInputValue('fullHtmlInput')"><i
                        class="ei-copy"></i></button>
            </div>
            <div class='input-w'>
                <input type="text" id='searchInput' class="ei-input" placeholder="Search icon.">
                <button class="ei-btn code-copy" title="切换模式" onclick="toggleMode(this)"><i class="ei-th"></i></button>
            </div>
        </div>
        <div id='no-icon'>没有找到查询结果</div>
        <ul class="clearfix" id="iconList">
            <li><i class="ei-resize"></i> <span>resize</span></li>
            <li><i class="ei-expand-full"></i> <span>expand-full</span></li>
            <li><i class="ei-collapse-full"></i> <span>collapse-full</span></li>
            <li><i class="ei-yinyang"></i> <span>yinyang</span></li>
            <li><i class="ei-window"></i> <span>window</span></li>
            <li><i class="ei-window-alt"></i> <span>window-alt</span></li>
            <li><i class="ei-carousel"></i> <span>carousel</span></li>
            <li><i class="ei-spinner-snake"></i> <span>spinner-snake</span></li>
            <li><i class="ei-spinner-indicator"></i> <span>spinner-indicator</span></li>
            <li><i class="ei-check-board"></i> <span>check-board</span></li>
            <li><i class="ei-bar-chart"></i> <span>bar-chart</span></li>
            <li><i class="ei-github"></i> <span>github</span></li>
            <li><i class="ei-dot-circle"></i> <span>dot-circle</span></li>
            <li><i class="ei-cube-alt"></i> <span>cube-alt</span></li>
            <li><i class="ei-cubes"></i> <span>cubes</span></li>
            <li><i class="ei-file-pdf"></i> <span>file-pdf</span></li>
            <li><i class="ei-file-word"></i> <span>file-word</span></li>
            <li><i class="ei-file-excel"></i> <span>file-excel</span></li>
            <li><i class="ei-file-powerpoint"></i> <span>file-powerpoint</span></li>
            <li><i class="ei-file-image"></i> <span>file-image</span></li>
            <li><i class="ei-file-archive"></i> <span>file-archive</span></li>
            <li><i class="ei-file-audio"></i> <span>file-audio</span></li>
            <li><i class="ei-file-movie"></i> <span>file-movie</span></li>
            <li><i class="ei-file-code"></i> <span>file-code</span></li>
            <li><i class="ei-circle-o-notch"></i> <span>circle-o-notch</span></li>
            <li><i class="ei-qq"></i> <span>qq</span></li>
            <li><i class="ei-wechat"></i> <span>wechat</span></li>
            <li><i class="ei-history"></i> <span>history</span></li>
            <li><i class="ei-circle-thin"></i> <span>circle-thin</span></li>
            <li><i class="ei-sliders"></i> <span>sliders</span></li>
            <li><i class="ei-newspaper-o"></i> <span>newspaper-o</span></li>
            <li><i class="ei-calculator"></i> <span>calculator</span></li>
            <li><i class="ei-paint-brush"></i> <span>paint-brush</span></li>
            <li><i class="ei-area-chart"></i> <span>area-chart</span></li>
            <li><i class="ei-pie-chart"></i> <span>pie-chart</span></li>
            <li><i class="ei-line-chart"></i> <span>line-chart</span></li>
            <li><i class="ei-toggle-off"></i> <span>toggle-off</span></li>
            <li><i class="ei-toggle-on"></i> <span>toggle-on</span></li>
            <li><i class="ei-diamond"></i> <span>diamond</span></li>
            <li><i class="ei-venus"></i> <span>venus</span></li>
            <li><i class="ei-mars"></i> <span>mars</span></li>
            <li><i class="ei-server"></i> <span>server</span></li>
            <li><i class="ei-music"></i> <span>music</span></li>
            <li><i class="ei-search"></i> <span>search</span></li>
            <li><i class="ei-envelope"></i> <span>envelope</span></li>
            <li><i class="ei-heart"></i> <span>heart</span></li>
            <li><i class="ei-star"></i> <span>star</span></li>
            <li><i class="ei-star-empty"></i> <span>star-empty</span></li>
            <li><i class="ei-user"></i> <span>user</span></li>
            <li><i class="ei-film"></i> <span>film</span></li>
            <li><i class="ei-th-large"></i> <span>th-large</span></li>
            <li><i class="ei-th"></i> <span>th</span></li>
            <li><i class="ei-th-list"></i> <span>th-list</span></li>
            <li><i class="ei-check"></i> <span>check</span></li>
            <li><i class="ei-times"></i> <span>times</span></li>
            <li><i class="ei-zoom-in"></i> <span>zoom-in</span></li>
            <li><i class="ei-zoom-out"></i> <span>zoom-out</span></li>
            <li><i class="ei-off"></i> <span>off</span></li>
            <li><i class="ei-cog"></i> <span>cog</span></li>
            <li><i class="ei-trash"></i> <span>trash</span></li>
            <li><i class="ei-home"></i> <span>home</span></li>
            <li><i class="ei-file-o"></i> <span>file-o</span></li>
            <li><i class="ei-time"></i> <span>time</span></li>
            <li><i class="ei-download-alt"></i> <span>download-alt</span></li>
            <li><i class="ei-download"></i> <span>download</span></li>
            <li><i class="ei-upload"></i> <span>upload</span></li>
            <li><i class="ei-inbox"></i> <span>inbox</span></li>
            <li><i class="ei-play-circle"></i> <span>play-circle</span></li>
            <li><i class="ei-repeat"></i> <span>repeat</span></li>
            <li><i class="ei-refresh"></i> <span>refresh</span></li>
            <li><i class="ei-list-alt"></i> <span>list-alt</span></li>
            <li><i class="ei-lock"></i> <span>lock</span></li>
            <li><i class="ei-flag"></i> <span>flag</span></li>
            <li><i class="ei-headphones"></i> <span>headphones</span></li>
            <li><i class="ei-volume-off"></i> <span>volume-off</span></li>
            <li><i class="ei-volume-up"></i> <span>volume-up</span></li>
            <li><i class="ei-qrcode"></i> <span>qrcode</span></li>
            <li><i class="ei-barcode"></i> <span>barcode</span></li>
            <li><i class="ei-tag"></i> <span>tag</span></li>
            <li><i class="ei-tags"></i> <span>tags</span></li>
            <li><i class="ei-book"></i> <span>book</span></li>
            <li><i class="ei-bookmark"></i> <span>bookmark</span></li>
            <li><i class="ei-print"></i> <span>print</span></li>
            <li><i class="ei-camera"></i> <span>camera</span></li>
            <li><i class="ei-font"></i> <span>font</span></li>
            <li><i class="ei-bold"></i> <span>bold</span></li>
            <li><i class="ei-italic"></i> <span>italic</span></li>
            <li><i class="ei-header"></i> <span>header</span></li>
            <li><i class="ei-underline"></i> <span>underline</span></li>
            <li><i class="ei-strikethrough"></i> <span>strikethrough</span></li>
            <li><i class="ei-eraser"></i> <span>eraser</span></li>
            <li><i class="ei-align-justify"></i> <span>align-justify</span></li>
            <li><i class="ei-align-left"></i> <span>align-left</span></li>
            <li><i class="ei-list"></i> <span>list</span></li>
            <li><i class="ei-picture"></i> <span>picture</span></li>
            <li><i class="ei-pencil"></i> <span>pencil</span></li>
            <li><i class="ei-map-marker"></i> <span>map-marker</span></li>
            <li><i class="ei-adjust"></i> <span>adjust</span></li>
            <li><i class="ei-tint"></i> <span>tint</span></li>
            <li><i class="ei-edit"></i> <span>edit</span></li>
            <li><i class="ei-share"></i> <span>share</span></li>
            <li><i class="ei-checked"></i> <span>checked</span></li>
            <li><i class="ei-arrows"></i> <span>arrows</span></li>
            <li><i class="ei-step-backward"></i> <span>step-backward</span></li>
            <li><i class="ei-fast-backward"></i> <span>fast-backward</span></li>
            <li><i class="ei-backward"></i> <span>backward</span></li>
            <li><i class="ei-play"></i> <span>play</span></li>
            <li><i class="ei-pause"></i> <span>pause</span></li>
            <li><i class="ei-stop"></i> <span>stop</span></li>
            <li><i class="ei-forward"></i> <span>forward</span></li>
            <li><i class="ei-fast-forward"></i> <span>fast-forward</span></li>
            <li><i class="ei-step-forward"></i> <span>step-forward</span></li>
            <li><i class="ei-eject"></i> <span>eject</span></li>
            <li><i class="ei-chevron-left"></i> <span>chevron-left</span></li>
            <li><i class="ei-chevron-right"></i> <span>chevron-right</span></li>
            <li><i class="ei-plus-sign"></i> <span>plus-sign</span></li>
            <li><i class="ei-minus-sign"></i> <span>minus-sign</span></li>
            <li><i class="ei-remove-sign"></i> <span>remove-sign</span></li>
            <li><i class="ei-check-circle"></i> <span>check-circle</span></li>
            <li><i class="ei-question-sign"></i> <span>question-sign</span></li>
            <li><i class="ei-info-sign"></i> <span>info-sign</span></li>
            <li><i class="ei-remove-circle"></i> <span>remove-circle</span></li>
            <li><i class="ei-check-circle-o"></i> <span>check-circle-o</span></li>
            <li><i class="ei-ban-circle"></i> <span>ban-circle</span></li>
            <li><i class="ei-arrow-left"></i> <span>arrow-left</span></li>
            <li><i class="ei-arrow-right"></i> <span>arrow-right</span></li>
            <li><i class="ei-arrow-up"></i> <span>arrow-up</span></li>
            <li><i class="ei-arrow-down"></i> <span>arrow-down</span></li>
            <li><i class="ei-share-alt"></i> <span>share-alt</span></li>
            <li><i class="ei-resize-full"></i> <span>resize-full</span></li>
            <li><i class="ei-resize-small"></i> <span>resize-small</span></li>
            <li><i class="ei-plus"></i> <span>plus</span></li>
            <li><i class="ei-minus"></i> <span>minus</span></li>
            <li><i class="ei-asterisk"></i> <span>asterisk</span></li>
            <li><i class="ei-exclamation-sign"></i> <span>exclamation-sign</span></li>
            <li><i class="ei-gift"></i> <span>gift</span></li>
            <li><i class="ei-leaf"></i> <span>leaf</span></li>
            <li><i class="ei-eye-open"></i> <span>eye-open</span></li>
            <li><i class="ei-eye-close"></i> <span>eye-close</span></li>
            <li><i class="ei-warning-sign"></i> <span>warning-sign</span></li>
            <li><i class="ei-plane"></i> <span>plane</span></li>
            <li><i class="ei-calendar"></i> <span>calendar</span></li>
            <li><i class="ei-random"></i> <span>random</span></li>
            <li><i class="ei-comment"></i> <span>comment</span></li>
            <li><i class="ei-chevron-up"></i> <span>chevron-up</span></li>
            <li><i class="ei-chevron-down"></i> <span>chevron-down</span></li>
            <li><i class="ei-shopping-cart"></i> <span>shopping-cart</span></li>
            <li><i class="ei-folder-close"></i> <span>folder-close</span></li>
            <li><i class="ei-folder-open"></i> <span>folder-open</span></li>
            <li><i class="ei-resize-v"></i> <span>resize-v</span></li>
            <li><i class="ei-resize-h"></i> <span>resize-h</span></li>
            <li><i class="ei-bar-chart-alt"></i> <span>bar-chart-alt</span></li>
            <li><i class="ei-camera-retro"></i> <span>camera-retro</span></li>
            <li><i class="ei-key"></i> <span>key</span></li>
            <li><i class="ei-cogs"></i> <span>cogs</span></li>
            <li><i class="ei-comments"></i> <span>comments</span></li>
            <li><i class="ei-thumbs-o-up"></i> <span>thumbs-o-up</span></li>
            <li><i class="ei-thumbs-o-down"></i> <span>thumbs-o-down</span></li>
            <li><i class="ei-star-half"></i> <span>star-half</span></li>
            <li><i class="ei-heart-empty"></i> <span>heart-empty</span></li>
            <li><i class="ei-signout"></i> <span>signout</span></li>
            <li><i class="ei-pushpin"></i> <span>pushpin</span></li>
            <li><i class="ei-external-link"></i> <span>external-link</span></li>
            <li><i class="ei-signin"></i> <span>signin</span></li>
            <li><i class="ei-trophy"></i> <span>trophy</span></li>
            <li><i class="ei-upload-alt"></i> <span>upload-alt</span></li>
            <li><i class="ei-lemon"></i> <span>lemon</span></li>
            <li><i class="ei-phone"></i> <span>phone</span></li>
            <li><i class="ei-check-empty"></i> <span>check-empty</span></li>
            <li><i class="ei-bookmark-empty"></i> <span>bookmark-empty</span></li>
            <li><i class="ei-phone-sign"></i> <span>phone-sign</span></li>
            <li><i class="ei-credit"></i> <span>credit</span></li>
            <li><i class="ei-rss"></i> <span>rss</span></li>
            <li><i class="ei-hdd"></i> <span>hdd</span></li>
            <li><i class="ei-bullhorn"></i> <span>bullhorn</span></li>
            <li><i class="ei-bell"></i> <span>bell</span></li>
            <li><i class="ei-certificate"></i> <span>certificate</span></li>
            <li><i class="ei-hand-right"></i> <span>hand-right</span></li>
            <li><i class="ei-hand-left"></i> <span>hand-left</span></li>
            <li><i class="ei-hand-up"></i> <span>hand-up</span></li>
            <li><i class="ei-hand-down"></i> <span>hand-down</span></li>
            <li><i class="ei-circle-arrow-left"></i> <span>circle-arrow-left</span></li>
            <li><i class="ei-circle-arrow-right"></i> <span>circle-arrow-right</span></li>
            <li><i class="ei-circle-arrow-up"></i> <span>circle-arrow-up</span></li>
            <li><i class="ei-circle-arrow-down"></i> <span>circle-arrow-down</span></li>
            <li><i class="ei-globe"></i> <span>globe</span></li>
            <li><i class="ei-wrench"></i> <span>wrench</span></li>
            <li><i class="ei-tasks"></i> <span>tasks</span></li>
            <li><i class="ei-filter"></i> <span>filter</span></li>
            <li><i class="ei-group"></i> <span>group</span></li>
            <li><i class="ei-link"></i> <span>link</span></li>
            <li><i class="ei-cloud"></i> <span>cloud</span></li>
            <li><i class="ei-beaker"></i> <span>beaker</span></li>
            <li><i class="ei-cut"></i> <span>cut</span></li>
            <li><i class="ei-copy"></i> <span>copy</span></li>
            <li><i class="ei-paper-clip"></i> <span>paper-clip</span></li>
            <li><i class="ei-save"></i> <span>save</span></li>
            <li><i class="ei-sign-blank"></i> <span>sign-blank</span></li>
            <li><i class="ei-bars"></i> <span>bars</span></li>
            <li><i class="ei-list-ul"></i> <span>list-ul</span></li>
            <li><i class="ei-list-ol"></i> <span>list-ol</span></li>
            <li><i class="ei-table"></i> <span>table</span></li>
            <li><i class="ei-magic"></i> <span>magic</span></li>
            <li><i class="ei-caret-down"></i> <span>caret-down</span></li>
            <li><i class="ei-caret-up"></i> <span>caret-up</span></li>
            <li><i class="ei-caret-left"></i> <span>caret-left</span></li>
            <li><i class="ei-caret-right"></i> <span>caret-right</span></li>
            <li><i class="ei-columns"></i> <span>columns</span></li>
            <li><i class="ei-sort"></i> <span>sort</span></li>
            <li><i class="ei-sort-down"></i> <span>sort-down</span></li>
            <li><i class="ei-sort-up"></i> <span>sort-up</span></li>
            <li><i class="ei-envelope-alt"></i> <span>envelope-alt</span></li>
            <li><i class="ei-undo"></i> <span>undo</span></li>
            <li><i class="ei-dashboard"></i> <span>dashboard</span></li>
            <li><i class="ei-comment-alt"></i> <span>comment-alt</span></li>
            <li><i class="ei-comments-alt"></i> <span>comments-alt</span></li>
            <li><i class="ei-bolt"></i> <span>bolt</span></li>
            <li><i class="ei-sitemap"></i> <span>sitemap</span></li>
            <li><i class="ei-umbrella"></i> <span>umbrella</span></li>
            <li><i class="ei-paste"></i> <span>paste</span></li>
            <li><i class="ei-lightbulb"></i> <span>lightbulb</span></li>
            <li><i class="ei-exchange"></i> <span>exchange</span></li>
            <li><i class="ei-cloud-download"></i> <span>cloud-download</span></li>
            <li><i class="ei-cloud-upload"></i> <span>cloud-upload</span></li>
            <li><i class="ei-bell-alt"></i> <span>bell-alt</span></li>
            <li><i class="ei-coffee"></i> <span>coffee</span></li>
            <li><i class="ei-file-text-o"></i> <span>file-text-o</span></li>
            <li><i class="ei-building"></i> <span>building</span></li>
            <li><i class="ei-double-angle-left"></i> <span>double-angle-left</span></li>
            <li><i class="ei-double-angle-right"></i> <span>double-angle-right</span></li>
            <li><i class="ei-double-angle-up"></i> <span>double-angle-up</span></li>
            <li><i class="ei-double-angle-down"></i> <span>double-angle-down</span></li>
            <li><i class="ei-angle-left"></i> <span>angle-left</span></li>
            <li><i class="ei-angle-right"></i> <span>angle-right</span></li>
            <li><i class="ei-angle-up"></i> <span>angle-up</span></li>
            <li><i class="ei-angle-down"></i> <span>angle-down</span></li>
            <li><i class="ei-desktop"></i> <span>desktop</span></li>
            <li><i class="ei-laptop"></i> <span>laptop</span></li>
            <li><i class="ei-tablet"></i> <span>tablet</span></li>
            <li><i class="ei-mobile"></i> <span>mobile</span></li>
            <li><i class="ei-circle-blank"></i> <span>circle-blank</span></li>
            <li><i class="ei-quote-left"></i> <span>quote-left</span></li>
            <li><i class="ei-quote-right"></i> <span>quote-right</span></li>
            <li><i class="ei-spinner"></i> <span>spinner</span></li>
            <li><i class="ei-circle"></i> <span>circle</span></li>
            <li><i class="ei-reply"></i> <span>reply</span></li>
            <li><i class="ei-folder-close-alt"></i> <span>folder-close-alt</span></li>
            <li><i class="ei-folder-open-alt"></i> <span>folder-open-alt</span></li>
            <li><i class="ei-expand-alt"></i> <span>expand-alt</span></li>
            <li><i class="ei-collapse-alt"></i> <span>collapse-alt</span></li>
            <li><i class="ei-smile"></i> <span>smile</span></li>
            <li><i class="ei-frown"></i> <span>frown</span></li>
            <li><i class="ei-meh"></i> <span>meh</span></li>
            <li><i class="ei-gamepad"></i> <span>gamepad</span></li>
            <li><i class="ei-keyboard"></i> <span>keyboard</span></li>
            <li><i class="ei-flag-alt"></i> <span>flag-alt</span></li>
            <li><i class="ei-flag-checkered"></i> <span>flag-checkered</span></li>
            <li><i class="ei-terminal"></i> <span>terminal</span></li>
            <li><i class="ei-code"></i> <span>code</span></li>
            <li><i class="ei-reply-all"></i> <span>reply-all</span></li>
            <li><i class="ei-star-half-full"></i> <span>star-half-full</span></li>
            <li><i class="ei-location-arrow"></i> <span>location-arrow</span></li>
            <li><i class="ei-crop"></i> <span>crop</span></li>
            <li><i class="ei-code-fork"></i> <span>code-fork</span></li>
            <li><i class="ei-unlink"></i> <span>unlink</span></li>
            <li><i class="ei-question"></i> <span>question</span></li>
            <li><i class="ei-info"></i> <span>info</span></li>
            <li><i class="ei-shield"></i> <span>shield</span></li>
            <li><i class="ei-calendar-empty"></i> <span>calendar-empty</span></li>
            <li><i class="ei-rocket"></i> <span>rocket</span></li>
            <li><i class="ei-chevron-sign-left"></i> <span>chevron-sign-left</span></li>
            <li><i class="ei-chevron-sign-right"></i> <span>chevron-sign-right</span></li>
            <li><i class="ei-chevron-sign-up"></i> <span>chevron-sign-up</span></li>
            <li><i class="ei-chevron-sign-down"></i> <span>chevron-sign-down</span></li>
            <li><i class="ei-html5"></i> <span>html5</span></li>
            <li><i class="ei-anchor"></i> <span>anchor</span></li>
            <li><i class="ei-unlock-alt"></i> <span>unlock-alt</span></li>
            <li><i class="ei-bullseye"></i> <span>bullseye</span></li>
            <li><i class="ei-ellipsis-h"></i> <span>ellipsis-h</span></li>
            <li><i class="ei-ellipsis-v"></i> <span>ellipsis-v</span></li>
            <li><i class="ei-rss-sign"></i> <span>rss-sign</span></li>
            <li><i class="ei-play-sign"></i> <span>play-sign</span></li>
            <li><i class="ei-minus-sign-alt"></i> <span>minus-sign-alt</span></li>
            <li><i class="ei-plus-sign-alt"></i> <span>plus-sign-alt</span></li>
            <li><i class="ei-check-minus"></i> <span>check-minus</span></li>
            <li><i class="ei-check-plus"></i> <span>check-plus</span></li>
            <li><i class="ei-level-up"></i> <span>level-up</span></li>
            <li><i class="ei-level-down"></i> <span>level-down</span></li>
            <li><i class="ei-check-sign"></i> <span>check-sign</span></li>
            <li><i class="ei-edit-sign"></i> <span>edit-sign</span></li>
            <li><i class="ei-external-link-sign"></i> <span>external-link-sign</span></li>
            <li><i class="ei-share-sign"></i> <span>share-sign</span></li>
            <li><i class="ei-compass"></i> <span>compass</span></li>
            <li><i class="ei-collapse"></i> <span>collapse</span></li>
            <li><i class="ei-collapse-top"></i> <span>collapse-top</span></li>
            <li><i class="ei-expand"></i> <span>expand</span></li>
            <li><i class="ei-dollar"></i> <span>dollar</span></li>
            <li><i class="ei-yen"></i> <span>yen</span></li>
            <li><i class="ei-file"></i> <span>file</span></li>
            <li><i class="ei-file-text"></i> <span>file-text</span></li>
            <li><i class="ei-sort-by-alphabet"></i> <span>sort-by-alphabet</span></li>
            <li><i class="ei-sort-by-alphabet-alt"></i> <span>sort-by-alphabet-alt</span></li>
            <li><i class="ei-sort-by-attributes"></i> <span>sort-by-attributes</span></li>
            <li><i class="ei-sort-by-attributes-alt"></i> <span>sort-by-attributes-alt</span></li>
            <li><i class="ei-sort-by-order"></i> <span>sort-by-order</span></li>
            <li><i class="ei-sort-by-order-alt"></i> <span>sort-by-order-alt</span></li>
            <li><i class="ei-thumbs-up"></i> <span>thumbs-up</span></li>
            <li><i class="ei-thumbs-down"></i> <span>thumbs-down</span></li>
            <li><i class="ei-long-arrow-down"></i> <span>long-arrow-down</span></li>
            <li><i class="ei-long-arrow-up"></i> <span>long-arrow-up</span></li>
            <li><i class="ei-long-arrow-left"></i> <span>long-arrow-left</span></li>
            <li><i class="ei-long-arrow-right"></i> <span>long-arrow-right</span></li>
            <li><i class="ei-apple"></i> <span>apple</span></li>
            <li><i class="ei-windows"></i> <span>windows</span></li>
            <li><i class="ei-android"></i> <span>android</span></li>
            <li><i class="ei-linux"></i> <span>linux</span></li>
            <li><i class="ei-sun"></i> <span>sun</span></li>
            <li><i class="ei-moon"></i> <span>moon</span></li>
            <li><i class="ei-archive"></i> <span>archive</span></li>
            <li><i class="ei-bug"></i> <span>bug</span></li>
            <li><i class="ei-zhifubao"></i> <span>zhifubao</span></li>
            <li><i class="ei-zhifubao-square"></i> <span>zhifubao-square</span></li>
            <li><i class="ei-taobao"></i> <span>taobao</span></li>
            <li><i class="ei-weibo"></i> <span>weibo</span></li>
            <li><i class="ei-renren"></i> <span>renren</span></li>
            <li><i class="ei-chrome"></i> <span>chrome</span></li>
            <li><i class="ei-firefox"></i> <span>firefox</span></li>
            <li><i class="ei-ie"></i> <span>ie</span></li>
            <li><i class="ei-opera"></i> <span>opera</span></li>
            <li><i class="ei-safari"></i> <span>safari</span></li>
            <li><i class="ei-node"></i> <span>node</span></li>
            <li><i class="ei-layout"></i> <span>layout</span></li>
            <li><i class="ei-usecase"></i> <span>usecase</span></li>
            <li><i class="ei-stack"></i> <span>stack</span></li>
            <li><i class="ei-branch"></i> <span>branch</span></li>
            <li><i class="ei-chat"></i> <span>chat</span></li>
            <li><i class="ei-chat-line"></i> <span>chat-line</span></li>
            <li><i class="ei-chat-dot"></i> <span>chat-dot</span></li>
            <li><i class="ei-cube"></i> <span>cube</span></li>
            <li><i class="ei-database"></i> <span>database</span></li>
            <li class="i-big"><i class="ei-chanzhi"></i> <span>chanzhi</span></li>
            <li class="i-big"><i class="ei-chanzhi-pro"></i> <span>chanzhi-pro</span></li>
            <li class="i-big"><i class="ei-zsite"></i> <span>zsite</span></li>
            <li class="i-big"><i class="ei-zsite-pro"></i> <span>zsite-pro</span></li>
        </ul>
    </div>
    <div id="no-icon" style="display: block;">Easy-ICON 使用 Font-Awesome 图标库, 对原作者做出的贡献表示感谢!</div>
    <div id='useBlock'>
        <div class="doc-title">如何使用?</div>
        <div class='doc-title-s'>1.安装</div>
        <div class='doc-text'>a.使用css文件引用:(推荐下载到本地然后引用本地文件)</div>
        <pre class='demo-code'>&lt;link rel="stylesheet" href="https://www.theajack.com/easy-icon/dist/easy-icon.min.css"></pre> 
        <div class='doc-text'>b.使用npm方式安装:</div>
        <pre class='demo-code'>npm i easy-icon</pre>
        <div class='doc-text'>您只需要引用一次即可:</div>
        <pre class='demo-code'>import 'easy-icon'</pre>
        <div class='doc-title-s'>2.使用</div>
        <div class='doc-text'>Easy ICON使用起来十分简单，您只需要在您想要使用的地方插入一个如下的标签即可:</div>
        <pre class='demo-code'>&lt;i class="ei-smile">&lt;/i></pre>
        <div class='doc-text'>然后您就可以看到一个可爱的图标: <i class="ei-smile"></i></div>
    </div>
    <div id='spinBlock'>
        <div class="doc-title">让图标旋转!</div>
        <div class='doc-text'>您可以通过添加 <span class="red">ei-spin</span> 类来使图标旋转:</div>
        <pre class='demo-code'>&lt;i class="ei-spinner-snake ei-spin">&lt;/i></pre>
        <div class='doc-text'>效果: <i class="ei-spinner-snake ei-spin"></i></div>
    </div>
    <div id='sizeBlock'>
        <div class="doc-title">选择尺寸</div>
        <div class='doc-text'>
            Easy ICON 内置了八种不同大小的尺寸，从小到大依次为:
            <span class="red">xs</span>,<span class="red">s</span>,<span class="red">l</span>,<span class="red">xl</span>,<span class="red">2x</span>,<span class="red">3x</span>,<span class="red">4x</span>,<span class="red">5x</span>
        </div>
<pre class='demo-code'>&lt;i class="ei-smile ei-xs">&lt;/i>
&lt;i class="ei-smile ei-s">&lt;/i>
&lt;i class="ei-smile ei-l">&lt;/i>
&lt;i class="ei-smile ei-xl">&lt;/i>
&lt;i class="ei-smile ei-2x">&lt;/i>
&lt;i class="ei-smile ei-3x">&lt;/i>
&lt;i class="ei-smile ei-4x">&lt;/i>
&lt;i class="ei-smile ei-5x">&lt;/i>
</pre>
        <div class='doc-text'>效果: <i class="ei-smile ei-xs"></i><i class="ei-smile ei-s"></i><i class="ei-smile ei-l"></i><i class="ei-smile ei-xl"></i><i class="ei-smile ei-2x"></i><i class="ei-smile ei-3x"></i><i class="ei-smile ei-4x"></i><i class="ei-smile ei-5x"></i></div>
        <div class='doc-text'>当然，您可以使用任何自定义css样式来覆盖默认的样式.</div>
    </div>
    <div id="footer" class="bg-black text-white part">
        <div id="footerLink">
            <a href='https://github.com/theajack' target="blank"><span class="link">GitHub</span></a>
            <span class="split-icon">|</span>
            <a href='http://weibo.com/p/1005055304330572/home?from=page_100505&amp;mod=TAB&amp;is_all=1' target="blank"><span class="link">新浪微博</span></a>
            <span class="split-icon">|</span>

            Email:theajack@qq.com
            <span class="split-icon d-hide">|</span>
            <a href='https://www.theajack.com' target="blank"><span class="link d-hide">theajack.com</span></a>
        </div>
        <div id="copyright">
            &copy; <span id="_year">2019</span> TheaJack All rights
            reserved
        </div>
    </div>
    <div id='toastEle'></div>
</body>

</html>