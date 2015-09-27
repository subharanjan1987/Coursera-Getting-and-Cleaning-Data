


<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=1020">
    
    
    <title>Coursera-Getting-and-Cleaning-Data/CodeBook.md at master · Xiaodan/Coursera-Getting-and-Cleaning-Data · GitHub</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="Xiaodan/Coursera-Getting-and-Cleaning-Data" name="twitter:title" /><meta content="Coursera-Getting-and-Cleaning-Data - Repo for Coursera.com online course: Getting and Cleaning Data" name="twitter:description" /><meta content="https://avatars3.githubusercontent.com/u/1871047?v=3&amp;s=400" name="twitter:image:src" />
      <meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars3.githubusercontent.com/u/1871047?v=3&amp;s=400" property="og:image" /><meta content="Xiaodan/Coursera-Getting-and-Cleaning-Data" property="og:title" /><meta content="https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data" property="og:url" /><meta content="Coursera-Getting-and-Cleaning-Data - Repo for Coursera.com online course: Getting and Cleaning Data" property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    
    <meta name="pjax-timeout" content="1000">
    

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
        <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="6A3313A4:0F68:1C9B3AE:5607F4A6" name="octolytics-dimension-request_id" />
    
    <meta content="Rails, view, blob#show" data-pjax-transient="true" name="analytics-event" />
    <meta class="js-ga-set" name="dimension1" content="Logged Out">
      <meta class="js-ga-set" name="dimension4" content="Current repo nav">
    <meta name="is-dotcom" content="true">
        <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <!-- </textarea> --><!-- '"` --><meta content="authenticity_token" name="csrf-param" />
<meta content="CtTRaA+6xOcav6ZGzNyc/fYST1QE3XefTN7uZJ9sHkCjHC4WKe0Uw/YtI4Y8xCcloiQKAb63jBUATAPsUeSwfg==" name="csrf-token" />
    

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-d3b5b3df2f65fc68f5e345a65ac963467f6c81cf28ea86808ec363627c646deb.css" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github2-5c5f822f8fcc71f3c7ef329235cc20ddb312d1e4a952030b5cbcce6bc6938888.css" media="all" rel="stylesheet" />
    
    


    <meta http-equiv="x-pjax-version" content="66f455c6719e9be482f1485001a46a01">

      
  <meta name="description" content="Coursera-Getting-and-Cleaning-Data - Repo for Coursera.com online course: Getting and Cleaning Data">
  <meta name="go-import" content="github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data git https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data.git">

  <meta content="1871047" name="octolytics-dimension-user_id" /><meta content="Xiaodan" name="octolytics-dimension-user_login" /><meta content="18748391" name="octolytics-dimension-repository_id" /><meta content="Xiaodan/Coursera-Getting-and-Cleaning-Data" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="18748391" name="octolytics-dimension-repository_network_root_id" /><meta content="Xiaodan/Coursera-Getting-and-Cleaning-Data" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data/commits/master.atom" rel="alternate" title="Recent Commits to Coursera-Getting-and-Cleaning-Data:master" type="application/atom+xml">

  </head>


  <body class="logged_out   env-production windows vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



      
      
      <div class="header header-logged-out" role="banner">
  <div class="container clearfix">

    <a class="header-logo-wordmark" href="https://github.com/" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
      <span class="mega-octicon octicon-logo-github"></span>
    </a>

    <div class="header-actions" role="navigation">
        <a class="btn btn-primary" href="/join" data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">Sign up</a>
      <a class="btn" href="/login?return_to=%2FXiaodan%2FCoursera-Getting-and-Cleaning-Data%2Fblob%2Fmaster%2Fpeer_assessment%2FCodeBook.md" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign in</a>
    </div>

    <div class="site-search repo-scope js-site-search" role="search">
      <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/Xiaodan/Coursera-Getting-and-Cleaning-Data/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/Xiaodan/Coursera-Getting-and-Cleaning-Data/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <label class="js-chromeless-input-container form-control">
    <div class="scope-badge">This repository</div>
    <input type="text"
      class="js-site-search-focus js-site-search-field is-clearable chromeless-input"
      data-hotkey="s"
      name="q"
      placeholder="Search"
      aria-label="Search this repository"
      data-global-scope-placeholder="Search GitHub"
      data-repo-scope-placeholder="Search"
      tabindex="1"
      autocapitalize="off">
  </label>
</form>
    </div>

      <ul class="header-nav left" role="navigation">
          <li class="header-nav-item">
            <a class="header-nav-link" href="/explore" data-ga-click="(Logged out) Header, go to explore, text:explore">Explore</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/features" data-ga-click="(Logged out) Header, go to features, text:features">Features</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="https://enterprise.github.com/" data-ga-click="(Logged out) Header, go to enterprise, text:enterprise">Enterprise</a>
          </li>
          <li class="header-nav-item">
            <a class="header-nav-link" href="/pricing" data-ga-click="(Logged out) Header, go to pricing, text:pricing">Pricing</a>
          </li>
      </ul>

  </div>
</div>



    <div id="start-of-content" class="accessibility-aid"></div>

    <div id="js-flash-container">
</div>


    <div role="main" class="main-content">
        <div itemscope itemtype="http://schema.org/WebPage">
    <div class="pagehead repohead instapaper_ignore readability-menu">

      <div class="container">

        <div class="clearfix">
          
<ul class="pagehead-actions">

  <li>
      <a href="/login?return_to=%2FXiaodan%2FCoursera-Getting-and-Cleaning-Data"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to watch a repository" rel="nofollow">
    <span class="octicon octicon-eye"></span>
    Watch
  </a>
  <a class="social-count" href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/watchers">
    7
  </a>

  </li>

  <li>
      <a href="/login?return_to=%2FXiaodan%2FCoursera-Getting-and-Cleaning-Data"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to star a repository" rel="nofollow">
    <span class="octicon octicon-star"></span>
    Star
  </a>

    <a class="social-count js-social-count" href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/stargazers">
      17
    </a>

  </li>

  <li>
      <a href="/login?return_to=%2FXiaodan%2FCoursera-Getting-and-Cleaning-Data"
        class="btn btn-sm btn-with-count tooltipped tooltipped-n"
        aria-label="You must be signed in to fork a repository" rel="nofollow">
        <span class="octicon octicon-repo-forked"></span>
        Fork
      </a>

    <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/network" class="social-count">
      192
    </a>
  </li>
</ul>

          <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public ">
  <span class="mega-octicon octicon-repo"></span>
  <span class="author"><a href="/Xiaodan" class="url fn" itemprop="url" rel="author"><span itemprop="title">Xiaodan</span></a></span><!--
--><span class="path-divider">/</span><!--
--><strong><a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data" data-pjax="#js-repo-pjax-container">Coursera-Getting-and-Cleaning-Data</a></strong>

  <span class="page-context-loader">
    <img alt="" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
  </span>

</h1>

        </div>
      </div>
    </div>

    <div class="container">
      <div class="repository-with-sidebar repo-container new-discussion-timeline ">
        <div class="repository-sidebar clearfix">
          
<nav class="sunken-menu repo-nav js-repo-nav js-sidenav-container-pjax js-octicon-loaders"
     role="navigation"
     data-pjax="#js-repo-pjax-container"
     data-issue-count-url="/Xiaodan/Coursera-Getting-and-Cleaning-Data/issues/counts">
  <ul class="sunken-menu-group">
    <li class="tooltipped tooltipped-w" aria-label="Code">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data" aria-label="Code" aria-selected="true" class="js-selected-navigation-item selected sunken-menu-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /Xiaodan/Coursera-Getting-and-Cleaning-Data">
        <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Issues">
        <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /Xiaodan/Coursera-Getting-and-Cleaning-Data/issues">
          <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
          <span class="js-issue-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

    <li class="tooltipped tooltipped-w" aria-label="Pull requests">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/pulls" aria-label="Pull requests" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g p" data-selected-links="repo_pulls /Xiaodan/Coursera-Getting-and-Cleaning-Data/pulls">
          <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull requests</span>
          <span class="js-pull-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

  </ul>
  <div class="sunken-menu-separator"></div>
  <ul class="sunken-menu-group">

    <li class="tooltipped tooltipped-w" aria-label="Pulse">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/pulse" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-selected-links="pulse /Xiaodan/Coursera-Getting-and-Cleaning-Data/pulse">
        <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

    <li class="tooltipped tooltipped-w" aria-label="Graphs">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-selected-links="repo_graphs repo_contributors /Xiaodan/Coursera-Getting-and-Cleaning-Data/graphs">
        <span class="octicon octicon-graph"></span> <span class="full-word">Graphs</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>
  </ul>


</nav>

            <div class="only-with-full-nav">
                
<div class="js-clone-url clone-url open"
  data-protocol-type="http">
  <h3><span class="text-emphasized">HTTPS</span> clone URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data.git" readonly="readonly" aria-label="HTTPS clone URL">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>

  
<div class="js-clone-url clone-url "
  data-protocol-type="subversion">
  <h3><span class="text-emphasized">Subversion</span> checkout URL</h3>
  <div class="input-group js-zeroclipboard-container">
    <input type="text" class="input-mini input-monospace js-url-field js-zeroclipboard-target"
           value="https://github.com/Xiaodan/Coursera-Getting-and-Cleaning-Data" readonly="readonly" aria-label="Subversion checkout URL">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>



<div class="clone-options">You can clone with
  <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone" class="inline-form js-clone-selector-form " data-form-nonce="0a739ad70309c0b850f218827d9c25968e24dc01" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="8CBrdK58uLXKmxgGngQ37pFgNSWdttmVqqmS/BQCBauPII7sVDdUFxGMk+1Gjm29OEyvrmmjQCpUi5A2BVuROQ==" /></div><button class="btn-link js-clone-selector" data-protocol="http" type="submit">HTTPS</button></form> or <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone" class="inline-form js-clone-selector-form " data-form-nonce="0a739ad70309c0b850f218827d9c25968e24dc01" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="bkgK+36h+OHfnXGA944IqbnOZ1ehQEJw8K7AMwcPpDW8/immyMPYakdPpW06EUtAmpyQtuhVM05MJv+SBMt4WA==" /></div><button class="btn-link js-clone-selector" data-protocol="subversion" type="submit">Subversion</button></form>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</div>
  <a href="https://windows.github.com" class="btn btn-sm sidebar-button" title="Save Xiaodan/Coursera-Getting-and-Cleaning-Data to your computer and use it in GitHub Desktop." aria-label="Save Xiaodan/Coursera-Getting-and-Cleaning-Data to your computer and use it in GitHub Desktop.">
    <span class="octicon octicon-desktop-download"></span>
    Clone in Desktop
  </a>

              <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/archive/master.zip"
                 class="btn btn-sm sidebar-button"
                 aria-label="Download the contents of Xiaodan/Coursera-Getting-and-Cleaning-Data as a zip file"
                 title="Download the contents of Xiaodan/Coursera-Getting-and-Cleaning-Data as a zip file"
                 rel="nofollow">
                <span class="octicon octicon-cloud-download"></span>
                Download ZIP
              </a>
            </div>
        </div>
        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>

          

<a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/blob/68b24d6a77de3f755e6ab37ec6515df6687c8536/peer_assessment/CodeBook.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:1c838d70baa99e432b4b8b9de42784f7 -->

  <div class="file-navigation js-zeroclipboard-container">
    
<div class="select-menu js-menu-container js-select-menu left">
  <span class="btn btn-sm select-menu-button js-menu-target css-truncate" data-hotkey="w"
    data-ref="master"
    title="master"
    role="button" aria-label="Switch branches or tags" tabindex="0" aria-haspopup="true">
    <i>Branch:</i>
    <span class="js-select-button css-truncate-target">master</span>
  </span>

  <div class="select-menu-modal-holder js-menu-content js-navigation-container" data-pjax aria-hidden="true">

    <div class="select-menu-modal">
      <div class="select-menu-header">
        <span class="select-menu-title">Switch branches/tags</span>
        <span class="octicon octicon-x js-menu-close" role="button" aria-label="Close"></span>
      </div>

      <div class="select-menu-filters">
        <div class="select-menu-text-filter">
          <input type="text" aria-label="Filter branches/tags" id="context-commitish-filter-field" class="js-filterable-field js-navigation-enable" placeholder="Filter branches/tags">
        </div>
        <div class="select-menu-tabs">
          <ul>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="branches" data-filter-placeholder="Filter branches/tags" class="js-select-menu-tab" role="tab">Branches</a>
            </li>
            <li class="select-menu-tab">
              <a href="#" data-tab-filter="tags" data-filter-placeholder="Find a tag…" class="js-select-menu-tab" role="tab">Tags</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="branches" role="menu">

        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


            <a class="select-menu-item js-navigation-item js-navigation-open selected"
               href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/blob/master/peer_assessment/CodeBook.md"
               data-name="master"
               data-skip-pjax="true"
               rel="nofollow">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <span class="select-menu-item-text css-truncate-target" title="master">
                master
              </span>
            </a>
        </div>

          <div class="select-menu-no-results">Nothing to show</div>
      </div>

      <div class="select-menu-list select-menu-tab-bucket js-select-menu-tab-bucket" data-tab-filter="tags">
        <div data-filterable-for="context-commitish-filter-field" data-filterable-type="substring">


        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

    <div class="btn-group right">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/find/master"
            class="js-show-file-finder btn btn-sm empty-icon tooltipped tooltipped-nw"
            data-pjax
            data-hotkey="t"
            aria-label="Quickly jump between files">
        <span class="octicon octicon-list-unordered"></span>
      </a>
      <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </div>

    <div class="breadcrumb js-zeroclipboard-target">
      <span class="repo-root js-repo-root"><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data" class="" data-branch="master" data-pjax="true" itemscope="url"><span itemprop="title">Coursera-Getting-and-Cleaning-Data</span></a></span></span><span class="separator">/</span><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/tree/master/peer_assessment" class="" data-branch="master" data-pjax="true" itemscope="url"><span itemprop="title">peer_assessment</span></a></span><span class="separator">/</span><strong class="final-path">CodeBook.md</strong>
    </div>
  </div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="@Xiaodan" class="avatar" height="24" src="https://avatars1.githubusercontent.com/u/1871047?v=3&amp;s=48" width="24" />
        <span class="author"><a href="/Xiaodan" rel="author">Xiaodan</a></span>
        <time datetime="2014-04-27T02:34:48Z" is="relative-time">Apr 26, 2014</time>
        <div class="commit-title">
            <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/commit/b03135c5c504c16cd5fcd27c26dd3b411bcd6660" class="message" data-pjax="true" title="added codebook.r">added codebook.r</a>
        </div>
    </div>

    <div class="participation">
      <p class="quickstat">
        <a href="#blob_contributors_box" rel="facebox">
          <strong>1</strong>
           contributor
        </a>
      </p>
      
    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header" data-facebox-id="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list" data-facebox-id="facebox-description">
          <li class="facebox-user-list-item">
            <img alt="@Xiaodan" height="24" src="https://avatars1.githubusercontent.com/u/1871047?v=3&amp;s=48" width="24" />
            <a href="/Xiaodan">Xiaodan</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="btn-group">
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/raw/master/peer_assessment/CodeBook.md" class="btn btn-sm " id="raw-url">Raw</a>
        <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/blame/master/peer_assessment/CodeBook.md" class="btn btn-sm js-update-url-with-hash">Blame</a>
      <a href="/Xiaodan/Coursera-Getting-and-Cleaning-Data/commits/master/peer_assessment/CodeBook.md" class="btn btn-sm " rel="nofollow">History</a>
    </div>

      <a class="octicon-btn tooltipped tooltipped-nw"
         href="https://windows.github.com"
         aria-label="Open this file in GitHub Desktop"
         data-ga-click="Repository, open with desktop, type:windows">
          <span class="octicon octicon-device-desktop"></span>
      </a>

        <button type="button" class="octicon-btn disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <span class="octicon octicon-pencil"></span>
        </button>
        <button type="button" class="octicon-btn octicon-btn-danger disabled tooltipped tooltipped-nw"
          aria-label="You must be signed in to make or propose changes">
          <span class="octicon octicon-trashcan"></span>
        </button>
  </div>

  <div class="file-info">
      22 lines (21 sloc)
      <span class="file-info-divider"></span>
    3.07 KB
  </div>
</div>

  
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1><a id="user-content-getting-and-cleaning-data-course-project-codebook" class="anchor" href="#getting-and-cleaning-data-course-project-codebook" aria-hidden="true"><span class="octicon octicon-link"></span></a>Getting and Cleaning Data Course Project CodeBook</h1>

<p>This file describes the variables, the data, and any transformations or work that I have performed to clean up the data.  </p>

<ul>
<li>The site where the data was obtained:<br>
<a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones">http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones</a><br>
The data for the project:<br>
<a href="https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip">https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip</a><br></li>
<li>The run_analysis.R script performs the following steps to clean the data:<br>

<ol>
<li>Read X_train.txt, y_train.txt and subject_train.txt from the "./data/train" folder and store them in <em>trainData</em>, <em>trainLabel</em> and <em>trainSubject</em> variables respectively.<br></li>
<li>Read X_test.txt, y_test.txt and subject_test.txt from the "./data/test" folder and store them in <em>testData</em>, <em>testLabel</em> and <em>testsubject</em> variables respectively.<br></li>
<li>Concatenate <em>testData</em> to <em>trainData</em> to generate a 10299x561 data frame, <em>joinData</em>; concatenate <em>testLabel</em> to <em>trainLabel</em> to generate a 10299x1 data frame, <em>joinLabel</em>; concatenate <em>testSubject</em> to <em>trainSubject</em> to generate a 10299x1 data frame, <em>joinSubject</em>.<br></li>
<li>Read the features.txt file from the "/data" folder and store the data in a variable called <em>features</em>. We only extract the measurements on the mean and standard deviation. This results in a 66 indices list. We get a subset of <em>joinData</em> with the 66 corresponding columns.<br></li>
<li>Clean the column names of the subset. We remove the "()" and "-" symbols in the names, as well as make the first letter of "mean" and "std" a capital letter "M" and "S" respectively.<br></li>
<li>Read the activity_labels.txt file from the "./data"" folder and store the data in a variable called <em>activity</em>.<br></li>
<li>Clean the activity names in the second column of <em>activity</em>. We first make all names to lower cases. If the name has an underscore between letters, we remove the underscore and capitalize the letter immediately after the underscore.<br></li>
<li>Transform the values of <em>joinLabel</em> according to the <em>activity</em> data frame.<br></li>
<li>Combine the <em>joinSubject</em>, <em>joinLabel</em> and <em>joinData</em> by column to get a new cleaned 10299x68 data frame, <em>cleanedData</em>. Properly name the first two columns, "subject" and "activity". The "subject" column contains integers that range from 1 to 30 inclusive; the "activity" column contains 6 kinds of activity names; the last 66 columns contain measurements that range from -1 to 1 exclusive.<br></li>
<li>Write the <em>cleanedData</em> out to "merged_data.txt" file in current working directory.<br></li>
<li>Finally, generate a second independent tidy data set with the average of each measurement for each activity and each subject. We have 30 unique subjects and 6 unique activities, which result in a 180 combinations of the two. Then, for each combination, we calculate the mean of each measurement with the corresponding combination. So, after initializing the <em>result</em> data frame and performing the two for-loops, we get a 180x68 data frame.</li>
<li>Write the <em>result</em> out to "data_with_means.txt" file in current working directory. </li>
</ol></li>
</ul>

<p>© Xiaodan Zhang 2014 All Rights reserved.</p>
</article>
  </div>

</div>

<a href="#jump-to-line" rel="facebox[.linejump]" data-hotkey="l" style="display:none">Jump to Line</a>
<div id="jump-to-line" style="display:none">
  <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="" class="js-jump-to-line-form" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
    <input class="linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
    <button type="submit" class="btn">Go</button>
</form></div>

        </div>
      </div>
      <div class="modal-backdrop"></div>
    </div>
  </div>


    </div>

      <div class="container">
  <div class="site-footer" role="contentinfo">
    <ul class="site-footer-links right">
        <li><a href="https://status.github.com/" data-ga-click="Footer, go to status, text:status">Status</a></li>
      <li><a href="https://developer.github.com" data-ga-click="Footer, go to api, text:api">API</a></li>
      <li><a href="https://training.github.com" data-ga-click="Footer, go to training, text:training">Training</a></li>
      <li><a href="https://shop.github.com" data-ga-click="Footer, go to shop, text:shop">Shop</a></li>
        <li><a href="https://github.com/blog" data-ga-click="Footer, go to blog, text:blog">Blog</a></li>
        <li><a href="https://github.com/about" data-ga-click="Footer, go to about, text:about">About</a></li>
        <li><a href="https://github.com/pricing" data-ga-click="Footer, go to pricing, text:pricing">Pricing</a></li>

    </ul>

    <a href="https://github.com" aria-label="Homepage">
      <span class="mega-octicon octicon-mark-github" title="GitHub"></span>
</a>
    <ul class="site-footer-links">
      <li>&copy; 2015 <span title="0.03929s from github-fe141-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
        <li><a href="https://github.com/site/terms" data-ga-click="Footer, go to terms, text:terms">Terms</a></li>
        <li><a href="https://github.com/site/privacy" data-ga-click="Footer, go to privacy, text:privacy">Privacy</a></li>
        <li><a href="https://github.com/security" data-ga-click="Footer, go to security, text:security">Security</a></li>
        <li><a href="https://github.com/contact" data-ga-click="Footer, go to contact, text:contact">Contact</a></li>
        <li><a href="https://help.github.com" data-ga-click="Footer, go to help, text:help">Help</a></li>
    </ul>
  </div>
</div>



    
    
    

    <div id="ajax-error-message" class="flash flash-error">
      <span class="octicon octicon-alert"></span>
      <button type="button" class="flash-close js-flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
        <span class="octicon octicon-x"></span>
      </button>
      Something went wrong with that request. Please try again.
    </div>


      <script crossorigin="anonymous" src="https://assets-cdn.github.com/assets/frameworks-f8473dece7242da6a20d52313634881b3975c52cebaa1e6c38157c0f26185691.js"></script>
      <script async="async" crossorigin="anonymous" src="https://assets-cdn.github.com/assets/github-ee6414bb0c9c43fe6c4b26b09ecaf335e6d76de02d92a150af292a1d2034b728.js"></script>
      
      
    <div class="js-stale-session-flash stale-session-flash flash flash-warn flash-banner hidden">
      <span class="octicon octicon-alert"></span>
      <span class="signed-in-tab-flash">You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
      <span class="signed-out-tab-flash">You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
    </div>
  </body>
</html>

