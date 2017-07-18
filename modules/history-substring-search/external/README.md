


<!DOCTYPE html>
<html lang="en" class="">
  <head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# object: http://ogp.me/ns/object# article: http://ogp.me/ns/article# profile: http://ogp.me/ns/profile#">
    <meta charset='utf-8'>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Content-Language" content="en">
    <meta name="viewport" content="width=1020">
    
    
    <title>zsh-history-substring-search/README.md at master · zsh-users/zsh-history-substring-search · GitHub</title>
    <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
    <link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
    <link rel="apple-touch-icon" sizes="57x57" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="114x114" href="/apple-touch-icon-114.png">
    <link rel="apple-touch-icon" sizes="72x72" href="/apple-touch-icon-144.png">
    <link rel="apple-touch-icon" sizes="144x144" href="/apple-touch-icon-144.png">
    <meta property="fb:app_id" content="1401488693436528">

      <meta content="@github" name="twitter:site" /><meta content="summary" name="twitter:card" /><meta content="zsh-users/zsh-history-substring-search" name="twitter:title" /><meta content="zsh-history-substring-search - ZSH port of Fish shell&#39;s history search feature." name="twitter:description" /><meta content="https://avatars3.githubusercontent.com/u/567410?v=3&amp;s=400" name="twitter:image:src" />
      <meta content="GitHub" property="og:site_name" /><meta content="object" property="og:type" /><meta content="https://avatars3.githubusercontent.com/u/567410?v=3&amp;s=400" property="og:image" /><meta content="zsh-users/zsh-history-substring-search" property="og:title" /><meta content="https://github.com/zsh-users/zsh-history-substring-search" property="og:url" /><meta content="zsh-history-substring-search - ZSH port of Fish shell&#39;s history search feature." property="og:description" />
      <meta name="browser-stats-url" content="https://api.github.com/_private/browser/stats">
    <meta name="browser-errors-url" content="https://api.github.com/_private/browser/errors">
    <link rel="assets" href="https://assets-cdn.github.com/">
    
    <meta name="pjax-timeout" content="1000">
    

    <meta name="msapplication-TileImage" content="/windows-tile.png">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="selected-link" value="repo_source" data-pjax-transient>

    <meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
        <meta name="google-analytics" content="UA-3769691-2">

    <meta content="collector.githubapp.com" name="octolytics-host" /><meta content="collector-cdn.github.com" name="octolytics-script-host" /><meta content="github" name="octolytics-app-id" /><meta content="586932C5:362E:4F7D6AE:5605AD6F" name="octolytics-dimension-request_id" />
    
    <meta content="Rails, view, blob#show" data-pjax-transient="true" name="analytics-event" />
    <meta class="js-ga-set" name="dimension1" content="Logged Out">
      <meta class="js-ga-set" name="dimension4" content="Current repo nav">
    <meta name="is-dotcom" content="true">
        <meta name="hostname" content="github.com">
    <meta name="user-login" content="">

      <link rel="mask-icon" href="https://assets-cdn.github.com/pinned-octocat.svg" color="#4078c0">
      <link rel="icon" type="image/x-icon" href="https://assets-cdn.github.com/favicon.ico">

    <!-- </textarea> --><!-- '"` --><meta content="authenticity_token" name="csrf-param" />
<meta content="yjT3OvCAKsSCQqj+uVJk+7v9WefkorukHy1w4vuMdFfUCv2SYo5dowILxExteaxeMfF9zuaZWZDz9p59p9khCw==" name="csrf-token" />
    

    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github-d3b5b3df2f65fc68f5e345a65ac963467f6c81cf28ea86808ec363627c646deb.css" media="all" rel="stylesheet" />
    <link crossorigin="anonymous" href="https://assets-cdn.github.com/assets/github2-5c5f822f8fcc71f3c7ef329235cc20ddb312d1e4a952030b5cbcce6bc6938888.css" media="all" rel="stylesheet" />
    
    


    <meta http-equiv="x-pjax-version" content="66f455c6719e9be482f1485001a46a01">

      
  <meta name="description" content="zsh-history-substring-search - ZSH port of Fish shell&#39;s history search feature.">
  <meta name="go-import" content="github.com/zsh-users/zsh-history-substring-search git https://github.com/zsh-users/zsh-history-substring-search.git">

  <meta content="567410" name="octolytics-dimension-user_id" /><meta content="zsh-users" name="octolytics-dimension-user_login" /><meta content="1808641" name="octolytics-dimension-repository_id" /><meta content="zsh-users/zsh-history-substring-search" name="octolytics-dimension-repository_nwo" /><meta content="true" name="octolytics-dimension-repository_public" /><meta content="false" name="octolytics-dimension-repository_is_fork" /><meta content="1808641" name="octolytics-dimension-repository_network_root_id" /><meta content="zsh-users/zsh-history-substring-search" name="octolytics-dimension-repository_network_root_nwo" />
  <link href="https://github.com/zsh-users/zsh-history-substring-search/commits/master.atom" rel="alternate" title="Recent Commits to zsh-history-substring-search:master" type="application/atom+xml">

  </head>


  <body class="logged_out   env-production  vis-public page-blob">
    <a href="#start-of-content" tabindex="1" class="accessibility-aid js-skip-to-content">Skip to content</a>

    
    
    



      
      
      <div class="header header-logged-out" role="banner">
  <div class="container clearfix">

    <a class="header-logo-wordmark" href="https://github.com/" data-ga-click="(Logged out) Header, go to homepage, icon:logo-wordmark">
      <span class="mega-octicon octicon-logo-github"></span>
    </a>

    <div class="header-actions" role="navigation">
        <a class="btn btn-primary" href="/join" data-ga-click="(Logged out) Header, clicked Sign up, text:sign-up">Sign up</a>
      <a class="btn" href="/login?return_to=%2Fzsh-users%2Fzsh-history-substring-search%2Fblob%2Fmaster%2FREADME.md" data-ga-click="(Logged out) Header, clicked Sign in, text:sign-in">Sign in</a>
    </div>

    <div class="site-search repo-scope js-site-search" role="search">
      <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/zsh-users/zsh-history-substring-search/search" class="js-site-search-form" data-global-search-url="/search" data-repo-search-url="/zsh-users/zsh-history-substring-search/search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
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
      <a href="/login?return_to=%2Fzsh-users%2Fzsh-history-substring-search"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to watch a repository" rel="nofollow">
    <span class="octicon octicon-eye"></span>
    Watch
  </a>
  <a class="social-count" href="/zsh-users/zsh-history-substring-search/watchers">
    20
  </a>

  </li>

  <li>
      <a href="/login?return_to=%2Fzsh-users%2Fzsh-history-substring-search"
    class="btn btn-sm btn-with-count tooltipped tooltipped-n"
    aria-label="You must be signed in to star a repository" rel="nofollow">
    <span class="octicon octicon-star"></span>
    Star
  </a>

    <a class="social-count js-social-count" href="/zsh-users/zsh-history-substring-search/stargazers">
      364
    </a>

  </li>

  <li>
      <a href="/login?return_to=%2Fzsh-users%2Fzsh-history-substring-search"
        class="btn btn-sm btn-with-count tooltipped tooltipped-n"
        aria-label="You must be signed in to fork a repository" rel="nofollow">
        <span class="octicon octicon-repo-forked"></span>
        Fork
      </a>

    <a href="/zsh-users/zsh-history-substring-search/network" class="social-count">
      34
    </a>
  </li>
</ul>

          <h1 itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="entry-title public ">
  <span class="mega-octicon octicon-repo"></span>
  <span class="author"><a href="/zsh-users" class="url fn" itemprop="url" rel="author"><span itemprop="title">zsh-users</span></a></span><!--
--><span class="path-divider">/</span><!--
--><strong><a href="/zsh-users/zsh-history-substring-search" data-pjax="#js-repo-pjax-container">zsh-history-substring-search</a></strong>

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
     data-issue-count-url="/zsh-users/zsh-history-substring-search/issues/counts">
  <ul class="sunken-menu-group">
    <li class="tooltipped tooltipped-w" aria-label="Code">
      <a href="/zsh-users/zsh-history-substring-search" aria-label="Code" aria-selected="true" class="js-selected-navigation-item selected sunken-menu-item" data-hotkey="g c" data-selected-links="repo_source repo_downloads repo_commits repo_releases repo_tags repo_branches /zsh-users/zsh-history-substring-search">
        <span class="octicon octicon-code"></span> <span class="full-word">Code</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

      <li class="tooltipped tooltipped-w" aria-label="Issues">
        <a href="/zsh-users/zsh-history-substring-search/issues" aria-label="Issues" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g i" data-selected-links="repo_issues repo_labels repo_milestones /zsh-users/zsh-history-substring-search/issues">
          <span class="octicon octicon-issue-opened"></span> <span class="full-word">Issues</span>
          <span class="js-issue-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>      </li>

    <li class="tooltipped tooltipped-w" aria-label="Pull requests">
      <a href="/zsh-users/zsh-history-substring-search/pulls" aria-label="Pull requests" class="js-selected-navigation-item sunken-menu-item" data-hotkey="g p" data-selected-links="repo_pulls /zsh-users/zsh-history-substring-search/pulls">
          <span class="octicon octicon-git-pull-request"></span> <span class="full-word">Pull requests</span>
          <span class="js-pull-replace-counter"></span>
          <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

  </ul>
  <div class="sunken-menu-separator"></div>
  <ul class="sunken-menu-group">

    <li class="tooltipped tooltipped-w" aria-label="Pulse">
      <a href="/zsh-users/zsh-history-substring-search/pulse" aria-label="Pulse" class="js-selected-navigation-item sunken-menu-item" data-selected-links="pulse /zsh-users/zsh-history-substring-search/pulse">
        <span class="octicon octicon-pulse"></span> <span class="full-word">Pulse</span>
        <img alt="" class="mini-loader" height="16" src="https://assets-cdn.github.com/images/spinners/octocat-spinner-32.gif" width="16" />
</a>    </li>

    <li class="tooltipped tooltipped-w" aria-label="Graphs">
      <a href="/zsh-users/zsh-history-substring-search/graphs" aria-label="Graphs" class="js-selected-navigation-item sunken-menu-item" data-selected-links="repo_graphs repo_contributors /zsh-users/zsh-history-substring-search/graphs">
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
           value="https://github.com/zsh-users/zsh-history-substring-search.git" readonly="readonly" aria-label="HTTPS clone URL">
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
           value="https://github.com/zsh-users/zsh-history-substring-search" readonly="readonly" aria-label="Subversion checkout URL">
    <span class="input-group-button">
      <button aria-label="Copy to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </span>
  </div>
</div>



<div class="clone-options">You can clone with
  <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/users/set_protocol?protocol_selector=http&amp;protocol_type=clone" class="inline-form js-clone-selector-form " data-form-nonce="b66753fd3c618bda7cbe0dbdd3e418728ed8ec8e" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="ywkGa7FzE4gvrrRl/vEPUmuDnw/hKeoLYDNxgjBOexv4EyohzIBdgVW2LkxzhJPxP3se2IIb92dkUVCU8iLXRQ==" /></div><button class="btn-link js-clone-selector" data-protocol="http" type="submit">HTTPS</button></form> or <!-- </textarea> --><!-- '"` --><form accept-charset="UTF-8" action="/users/set_protocol?protocol_selector=subversion&amp;protocol_type=clone" class="inline-form js-clone-selector-form " data-form-nonce="b66753fd3c618bda7cbe0dbdd3e418728ed8ec8e" data-remote="true" method="post"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /><input name="authenticity_token" type="hidden" value="5PQJjs6WyfnbCblQzU7Qs2sEm03Ru6SXJS4ZWwxsQkMErlFRqw1RKAm07bct85JCpcCTrkXvBKt5B8oHpnfF9A==" /></div><button class="btn-link js-clone-selector" data-protocol="subversion" type="submit">Subversion</button></form>.
  <a href="https://help.github.com/articles/which-remote-url-should-i-use" class="help tooltipped tooltipped-n" aria-label="Get help on which URL is right for you.">
    <span class="octicon octicon-question"></span>
  </a>
</div>

              <a href="/zsh-users/zsh-history-substring-search/archive/master.zip"
                 class="btn btn-sm sidebar-button"
                 aria-label="Download the contents of zsh-users/zsh-history-substring-search as a zip file"
                 title="Download the contents of zsh-users/zsh-history-substring-search as a zip file"
                 rel="nofollow">
                <span class="octicon octicon-cloud-download"></span>
                Download ZIP
              </a>
            </div>
        </div>
        <div id="js-repo-pjax-container" class="repository-content context-loader-container" data-pjax-container>

          

<a href="/zsh-users/zsh-history-substring-search/blob/c4a83561a12b898ff7145856d0e6ae50757e28ba/README.md" class="hidden js-permalink-shortcut" data-hotkey="y">Permalink</a>

<!-- blob contrib key: blob_contributors:v21:4a8ccd5ad0f23a13745cf0cc394700f9 -->

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
               href="/zsh-users/zsh-history-substring-search/blob/master/README.md"
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


            <div class="select-menu-item js-navigation-item ">
              <span class="select-menu-item-icon octicon octicon-check"></span>
              <a href="/zsh-users/zsh-history-substring-search/tree/v1.0.0/README.md"
                 data-name="v1.0.0"
                 data-skip-pjax="true"
                 rel="nofollow"
                 class="js-navigation-open select-menu-item-text css-truncate-target"
                 title="v1.0.0">v1.0.0</a>
            </div>
        </div>

        <div class="select-menu-no-results">Nothing to show</div>
      </div>

    </div>
  </div>
</div>

    <div class="btn-group right">
      <a href="/zsh-users/zsh-history-substring-search/find/master"
            class="js-show-file-finder btn btn-sm empty-icon tooltipped tooltipped-nw"
            data-pjax
            data-hotkey="t"
            aria-label="Quickly jump between files">
        <span class="octicon octicon-list-unordered"></span>
      </a>
      <button aria-label="Copy file path to clipboard" class="js-zeroclipboard btn btn-sm zeroclipboard-button tooltipped tooltipped-s" data-copied-hint="Copied!" type="button"><span class="octicon octicon-clippy"></span></button>
    </div>

    <div class="breadcrumb js-zeroclipboard-target">
      <span class="repo-root js-repo-root"><span itemscope="" itemtype="http://data-vocabulary.org/Breadcrumb"><a href="/zsh-users/zsh-history-substring-search" class="" data-branch="master" data-pjax="true" itemscope="url"><span itemprop="title">zsh-history-substring-search</span></a></span></span><span class="separator">/</span><strong class="final-path">README.md</strong>
    </div>
  </div>


  <div class="commit file-history-tease">
    <div class="file-history-tease-header">
        <img alt="@sunaku" class="avatar" height="24" src="https://avatars3.githubusercontent.com/u/9863?v=3&amp;s=48" width="24" />
        <span class="author"><a href="/sunaku" rel="contributor">sunaku</a></span>
        <time datetime="2015-04-27T03:17:10Z" is="relative-time">Apr 26, 2015</time>
        <div class="commit-title">
            <a href="/zsh-users/zsh-history-substring-search/commit/c4a83561a12b898ff7145856d0e6ae50757e28ba" class="message" data-pjax="true" title="README: add Fedora 21 to fallback up/down bindkey

https://github.com/zsh-users/zsh-history-substring-search/issues/37#issuecomment-96327615">README: add Fedora 21 to fallback up/down bindkey</a>
        </div>
    </div>

    <div class="participation">
      <p class="quickstat">
        <a href="#blob_contributors_box" rel="facebox">
          <strong>5</strong>
           contributors
        </a>
      </p>
          <a class="avatar-link tooltipped tooltipped-s" aria-label="sunaku" href="/zsh-users/zsh-history-substring-search/commits/master/README.md?author=sunaku"><img alt="@sunaku" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/9863?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="sorin-ionescu" href="/zsh-users/zsh-history-substring-search/commits/master/README.md?author=sorin-ionescu"><img alt="@sorin-ionescu" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/93816?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="Tarrasch" href="/zsh-users/zsh-history-substring-search/commits/master/README.md?author=Tarrasch"><img alt="@Tarrasch" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/294349?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="lonepie" href="/zsh-users/zsh-history-substring-search/commits/master/README.md?author=lonepie"><img alt="@lonepie" class="avatar" height="20" src="https://avatars1.githubusercontent.com/u/67245?v=3&amp;s=40" width="20" /> </a>
    <a class="avatar-link tooltipped tooltipped-s" aria-label="joe9" href="/zsh-users/zsh-history-substring-search/commits/master/README.md?author=joe9"><img alt="@joe9" class="avatar" height="20" src="https://avatars3.githubusercontent.com/u/1084520?v=3&amp;s=40" width="20" /> </a>


    </div>
    <div id="blob_contributors_box" style="display:none">
      <h2 class="facebox-header" data-facebox-id="facebox-header">Users who have contributed to this file</h2>
      <ul class="facebox-user-list" data-facebox-id="facebox-description">
          <li class="facebox-user-list-item">
            <img alt="@sunaku" height="24" src="https://avatars3.githubusercontent.com/u/9863?v=3&amp;s=48" width="24" />
            <a href="/sunaku">sunaku</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@sorin-ionescu" height="24" src="https://avatars3.githubusercontent.com/u/93816?v=3&amp;s=48" width="24" />
            <a href="/sorin-ionescu">sorin-ionescu</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@Tarrasch" height="24" src="https://avatars1.githubusercontent.com/u/294349?v=3&amp;s=48" width="24" />
            <a href="/Tarrasch">Tarrasch</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@lonepie" height="24" src="https://avatars3.githubusercontent.com/u/67245?v=3&amp;s=48" width="24" />
            <a href="/lonepie">lonepie</a>
          </li>
          <li class="facebox-user-list-item">
            <img alt="@joe9" height="24" src="https://avatars1.githubusercontent.com/u/1084520?v=3&amp;s=48" width="24" />
            <a href="/joe9">joe9</a>
          </li>
      </ul>
    </div>
  </div>

<div class="file">
  <div class="file-header">
  <div class="file-actions">

    <div class="btn-group">
      <a href="/zsh-users/zsh-history-substring-search/raw/master/README.md" class="btn btn-sm " id="raw-url">Raw</a>
        <a href="/zsh-users/zsh-history-substring-search/blame/master/README.md" class="btn btn-sm js-update-url-with-hash">Blame</a>
      <a href="/zsh-users/zsh-history-substring-search/commits/master/README.md" class="btn btn-sm " rel="nofollow">History</a>
    </div>


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
      128 lines (96 sloc)
      <span class="file-info-divider"></span>
    5.93 KB
  </div>
</div>

  
  <div id="readme" class="blob instapaper_body">
    <article class="markdown-body entry-content" itemprop="mainContentOfPage"><h1><a id="user-content-zsh-history-substring-search" class="anchor" href="#zsh-history-substring-search" aria-hidden="true"><span class="octicon octicon-link"></span></a>zsh-history-substring-search</h1>

<p>This is a clean-room implementation of the <a href="http://fishshell.com">Fish shell</a>'s history search
feature, where you can type in any part of any previously entered command
and press the UP and DOWN arrow keys to cycle through the matching commands.
You can also use K and J in VI mode or ^P and ^N in EMACS mode for the same.</p>

<hr>

<h2><a id="user-content-requirements" class="anchor" href="#requirements" aria-hidden="true"><span class="octicon octicon-link"></span></a>Requirements</h2>

<ul>
<li><a href="http://zsh.sourceforge.net">ZSH</a> 4.3 or newer</li>
</ul>

<hr>

<h2><a id="user-content-usage" class="anchor" href="#usage" aria-hidden="true"><span class="octicon octicon-link"></span></a>Usage</h2>

<ol>
<li><p>Load this script into your interactive ZSH session:</p>

<pre><code>% source zsh-history-substring-search.zsh
</code></pre>

<p>If you want to use <a href="https://github.com/zsh-users/zsh-syntax-highlighting">zsh-syntax-highlighting</a> along with this script,
then make sure that you load it <em>before</em> you load this script:</p>

<pre><code>% source zsh-syntax-highlighting.zsh
% source zsh-history-substring-search.zsh
</code></pre></li>
<li><p>Bind keyboard shortcuts to this script's functions:</p>

<pre><code># bind UP and DOWN arrow keys
zmodload zsh/terminfo
bindkey "$terminfo[kcuu1]" history-substring-search-up
bindkey "$terminfo[kcud1]" history-substring-search-down

# bind UP and DOWN arrow keys (compatibility fallback
# for Ubuntu 12.04, Fedora 21, and MacOSX 10.9 users)
bindkey '^[[A' history-substring-search-up
bindkey '^[[B' history-substring-search-down

# bind P and N for EMACS mode
bindkey -M emacs '^P' history-substring-search-up
bindkey -M emacs '^N' history-substring-search-down

# bind k and j for VI mode
bindkey -M vicmd 'k' history-substring-search-up
bindkey -M vicmd 'j' history-substring-search-down
</code></pre></li>
<li><p>Type any part of any previous command and then:</p>

<ul>
<li><p>Press the UP arrow key to select the nearest command that (1) contains
your query and (2) is older than the current command in the command
history.</p></li>
<li><p>Press the DOWN arrow key to select the nearest command that (1)
contains your query and (2) is newer than the current command in the
command history.</p></li>
<li><p>Press ^U (the Control and U keys simultaneously) to abort the search.</p></li>
</ul></li>
<li><p>If a matching command spans more than one line of text, press the LEFT
arrow key to move the cursor away from the end of the command, and then:</p>

<ul>
<li><p>Press the UP arrow key to move the cursor to the line above.  When the
cursor reaches the first line of the command, pressing the UP arrow
key again will cause this script to perform another search.</p></li>
<li><p>Press the DOWN arrow key to move the cursor to the line below.  When
the cursor reaches the last line of the command, pressing the DOWN
arrow key again will cause this script to perform another search.</p></li>
</ul></li>
</ol>

<hr>

<h2><a id="user-content-configuration" class="anchor" href="#configuration" aria-hidden="true"><span class="octicon octicon-link"></span></a>Configuration</h2>

<p>This script defines the following global variables. You may override their
default values only after having loaded this script into your ZSH session.</p>

<ul>
<li><p>HISTORY_SUBSTRING_SEARCH_HIGHLIGHT_FOUND is a global variable that defines
how the query should be highlighted inside a matching command. Its default
value causes this script to highlight using bold, white text on a magenta
background. See the "Character Highlighting" section in the zshzle(1) man
page to learn about the kinds of values you may assign to this variable.</p></li>
<li><p>HISTORY_SUBSTRING_SEARCH_HIGHLIGHT_NOT_FOUND is a global variable that
defines how the query should be highlighted when no commands in the
history match it. Its default value causes this script to highlight using
bold, white text on a red background. See the "Character Highlighting"
section in the zshzle(1) man page to learn about the kinds of values you
may assign to this variable.</p></li>
<li><p>HISTORY_SUBSTRING_SEARCH_GLOBBING_FLAGS is a global variable that defines
how the command history will be searched for your query. Its default value
causes this script to perform a case-insensitive search. See the "Globbing
Flags" section in the zshexpn(1) man page to learn about the kinds of
values you may assign to this variable.</p></li>
</ul>

<p>To always receive <em>unique</em> search results, use <code>setopt HIST_IGNORE_ALL_DUPS</code>.
Alternatively, use <code>setopt HIST_FIND_NO_DUPS</code> which makes this plugin skip
duplicate <em>adjacent</em> search results as you cycle through them---however, this
does not guarantee that search results are unique: if your search results were
"Dog", "Dog", "HotDog", "Dog", then cycling them gives "Dog", "HotDog", "Dog".
Notice that the "Dog" search result appeared twice as you cycled through them!
If you wish to avoid this limitation, then use <code>setopt HIST_IGNORE_ALL_DUPS</code>.</p>

<hr>

<h2><a id="user-content-history" class="anchor" href="#history" aria-hidden="true"><span class="octicon octicon-link"></span></a>History</h2>

<p>This script was originally written by <a href="http://www.zsh.org/mla/users/2009/msg00818.html">Peter Stephenson</a>, who published it
to the ZSH users mailing list (thereby making it public domain) in September
2009. It was later revised by Guido van Steen and released under the BSD
license (see below) as part of <a href="http://sourceforge.net/projects/fizsh/">the fizsh project</a> in January 2011.</p>

<p>It was later extracted from fizsh release 1.0.1, refactored heavily, and
repackaged as both an <a href="https://github.com/robbyrussell/oh-my-zsh/pull/215">oh-my-zsh plugin</a> and as an independently loadable
<a href="https://github.com/zsh-users/zsh-history-substring-search">ZSH script</a> by Suraj N. Kurapati in 2011.</p>

<p>It was <a href="https://github.com/robbyrussell/oh-my-zsh/pull/215">further developed</a> by Guido van Steen, Suraj N. Kurapati, Sorin
Ionescu, and Vincent Guerci in 2011.</p>
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
      <li>&copy; 2015 <span title="0.05299s from github-fe132-cp1-prd.iad.github.net">GitHub</span>, Inc.</li>
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

