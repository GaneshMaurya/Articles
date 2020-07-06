<!DOCTYPE html>
<!-- saved from url=(0097)https://www.freecodecamp.org/news/how-to-build-and-train-k-nearest-neighbors-ml-models-in-python/ -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">

    
    <meta http-equiv="X-UA-Compatible" content="IE=edge">

    <title>How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python</title>
    <meta name="HandheldFriendly" content="True">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <link rel="stylesheet" type="text/css" href="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism.min.css">
    <link rel="stylesheet" type="text/css" href="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-unescaped-markup.css">

    <link href="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/css" rel="stylesheet">

    <link rel="stylesheet" type="text/css" href="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/screen.css">
    <link rel="stylesheet" type="text/css" href="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/algolia-search.css">

    <script type="text/javascript" async="" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/analytics.js.download"></script><script src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/algoliasearch.min.js.download"></script>
    <script src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/autocomplete.min.js.download"></script>

    <script src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/saved_resource"></script>

    <link rel="shortcut icon" href="https://www.freecodecamp.org/news/favicon.png" type="image/png">
    <link rel="canonical" href="https://www.freecodecamp.org/news/how-to-build-and-train-k-nearest-neighbors-ml-models-in-python/">
    <meta name="referrer" content="no-referrer-when-downgrade">
    <link rel="amphtml" href="https://www.freecodecamp.org/news/how-to-build-and-train-k-nearest-neighbors-ml-models-in-python/amp/">
    
    <meta property="og:site_name" content="freeCodeCamp.org">
    <meta property="og:type" content="article">
    <meta property="og:title" content="How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python">
    <meta property="og:description" content="One of machine learning&#39;s most popular applications
[https://gumroad.com/l/pGjwd] is in solving classification problems.

Classification problems are situations where you have a data set, and you want
to classify observations from that data set into a specific category. 

A famous example is a spam filter for email providers. Gmail uses supervised
machine learning techniques to automatically place emails in your spam folder
based on their content, subject line, and other features.

Two machine l">
    <meta property="og:url" content="https://www.freecodecamp.org/news/how-to-build-and-train-k-nearest-neighbors-ml-models-in-python/">
    <meta property="og:image" content="https://www.freecodecamp.org/news/content/images/2020/07/classificaton.png">
    <meta property="article:published_time" content="2020-07-03T19:40:58.000Z">
    <meta property="article:modified_time" content="2020-07-06T06:48:45.000Z">
    <meta property="article:tag" content="Machine Learning">
    <meta property="article:tag" content="Python">
    
    <meta property="article:publisher" content="https://www.facebook.com/freecodecamp">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python">
    <meta name="twitter:description" content="One of machine learning&#39;s most popular applications
[https://gumroad.com/l/pGjwd] is in solving classification problems.

Classification problems are situations where you have a data set, and you want
to classify observations from that data set into a specific category. 

A famous example is a spam filter for email providers. Gmail uses supervised
machine learning techniques to automatically place emails in your spam folder
based on their content, subject line, and other features.

Two machine l">
    <meta name="twitter:url" content="https://www.freecodecamp.org/news/how-to-build-and-train-k-nearest-neighbors-ml-models-in-python/">
    <meta name="twitter:image" content="https://www.freecodecamp.org/news/content/images/2020/07/classificaton.png">
    <meta name="twitter:label1" content="Written by">
    <meta name="twitter:data1" content="Nick McCullum">
    <meta name="twitter:label2" content="Filed under">
    <meta name="twitter:data2" content="Machine Learning, Python">
    <meta name="twitter:site" content="@freecodecamp">
    <meta name="twitter:creator" content="@NickJMcCullum">
    <meta property="og:image:width" content="377">
    <meta property="og:image:height" content="248">
    
    <script type="application/ld+json">
{
    "@context": "https://schema.org",
    "@type": "Article",
    "publisher": {
        "@type": "Organization",
        "name": "freeCodeCamp.org",
        "logo": {
            "@type": "ImageObject",
            "url": "https://www.freecodecamp.org/news/content/images/2019/11/fcc_primary_large_24X210.svg",
            "width": 210,
            "height": 24
        }
    },
    "author": {
        "@type": "Person",
        "name": "Nick McCullum",
        "image": {
            "@type": "ImageObject",
            "url": "https://www.freecodecamp.org/news/content/images/2020/04/0Y2A0586-2.jpg",
            "width": 2000,
            "height": 2001
        },
        "url": "https://www.freecodecamp.org/news/author/nick/",
        "sameAs": [
            "http://nickmccullum.com",
            "https://twitter.com/NickJMcCullum"
        ]
    },
    "headline": "How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python",
    "url": "https://www.freecodecamp.org/news/how-to-build-and-train-k-nearest-neighbors-ml-models-in-python/",
    "datePublished": "2020-07-03T19:40:58.000Z",
    "dateModified": "2020-07-06T06:48:45.000Z",
    "image": {
        "@type": "ImageObject",
        "url": "https://www.freecodecamp.org/news/content/images/2020/07/classificaton.png",
        "width": 377,
        "height": 248
    },
    "keywords": "Machine Learning, Python",
    "description": "One of machine learning&#x27;s most popular applications\n[https://gumroad.com/l/pGjwd] is in solving classification problems.\n\nClassification problems are situations where you have a data set, and you want\nto classify observations from that data set into a specific category. \n\nA famous example is a spam filter for email providers. Gmail uses supervised\nmachine learning techniques to automatically place emails in your spam folder\nbased on their content, subject line, and other features.\n\nTwo machine l",
    "mainEntityOfPage": {
        "@type": "WebPage",
        "@id": "https://www.freecodecamp.org/news/"
    }
}
    </script>

    <meta name="generator" content="Ghost 2.37">
    <link rel="alternate" type="application/rss+xml" title="freeCodeCamp.org" href="https://www.freecodecamp.org/news/rss/">

<style id="fit-vids-style">.fluid-width-video-container{flex-grow: 1;width:100%;}.fluid-width-video-wrapper{width:100%;position:relative;padding:0;}.fluid-width-video-wrapper iframe,.fluid-width-video-wrapper object,.fluid-width-video-wrapper embed {position:absolute;top:0;left:0;width:100%;height:100%;}</style></head>

<body class="post-template tag-machine-learning tag-python" data-gr-c-s-loaded="true">

    <div class="site-wrapper">
        <nav class="site-nav nav-padding">
    <div class="site-nav-left">
        <form id="search-form" onsubmit="submitSearch()">
  <div role="search" class="searchbox__wrapper">
    <span class="algolia-autocomplete" style="position: relative; display: inline-block; direction: ltr;"><input type="search" placeholder="Search 6,000+ tutorials" id="search-input" class="aa-input" autocomplete="off" spellcheck="false" role="combobox" aria-autocomplete="list" aria-expanded="false" aria-owns="algolia-autocomplete-listbox-0" dir="auto" style="position: relative; vertical-align: top;"><pre aria-hidden="true" style="position: absolute; visibility: hidden; white-space: pre; font-family: Lato, sans-serif; font-size: 18px; font-style: normal; font-variant: normal; font-weight: 400; word-spacing: 0px; letter-spacing: normal; text-indent: 0px; text-rendering: auto; text-transform: none;"></pre><span class="aa-dropdown-menu" role="listbox" id="algolia-autocomplete-listbox-0" style="position: absolute; top: 100%; z-index: 100; display: none; left: 0px; right: auto;"><div class="aa-dataset-1"></div></span></span>
    <button type="submit" title="Submit your search query." class="ais-SearchBox-submit">
      <svg class="ais-SearchBox-submitIcon" xmlns="http://www.w3.org/2000/svg" width="10" height="10" viewBox="0 0 40 40">
        <path d="M26.804 29.01c-2.832 2.34-6.465 3.746-10.426 3.746C7.333 32.756 0 25.424 0 16.378 0 7.333 7.333 0 16.378 0c9.046 0 16.378 7.333 16.378 16.378 0 3.96-1.406 7.594-3.746 10.426l10.534 10.534c.607.607.61 1.59-.004 2.202-.61.61-1.597.61-2.202.004L26.804 29.01zm-10.426.627c7.323 0 13.26-5.936 13.26-13.26 0-7.32-5.937-13.257-13.26-13.257C9.056 3.12 3.12 9.056 3.12 16.378c0 7.323 5.936 13.26 13.258 13.26z"></path>
      </svg>
    </button>
  </div>
</form>

<script>
  const client = algoliasearch('QMJYL5WYTI', '4318af87aa3ce128708f1153556c6108');
  const index = client.initIndex('news');
  const screenWidth = window.screen.width;
  const screenHeight = window.screen.height;
  const hitsToRender = (screenWidth >= 767 && screenHeight >= 768) ? 8 : 5;
  autocomplete('#search-input', { 
      hint: false,
      keyboardShortcuts: ['s', 191]
    }, [
    {
      source: autocomplete.sources.hits(index, { hitsPerPage: hitsToRender }),
      debounce: 250,
      templates: {
        suggestion: (suggestion, result) => {
          hits = true;
          return `
            <a href="${suggestion.url}">
              <div class="algolia-result">
                <span>${suggestion._highlightResult.title.value}</span>
              </div>
            </a>
          `;
        },
        empty: (options) => {
          hits = false;
          return `
            <div class="aa-suggestion footer-suggestion no-hits-footer">
              <div class="algolia-result">
                <span>
                  No tutorials found
                </span>
              </div>
            </div>
          `;
        },
        footer: (query, result) => {
          if (!query.isEmpty) {
            return `
              <div class="aa-suggestion footer-suggestion">
                <a id="algolia-footer-selector" href="https://www.freecodecamp.org/news/search?query=${result.query}">
                  <div class="algolia-result algolia-footer">
                    <span>See all results for ${result.query}</span>
                  </div>
                </a>
              </div>
            `;
          }
        }
      }
    }
  ]).on('autocomplete:closed', () => {
    // Clicked off dropdown or pressed Esc key
    hits = false;
  }).on('autocomplete:selected', (event, suggestion, dataset, context) => {
    // Set to hit URL if hit is selected by mouse click or enter key
    hitSelected = suggestion.url;
    // Do nothing on click, as the browser will already do it
    if (context.selectionMethod === 'click') {
      return;
    }
    // Change the page, for example, on other events
    window.location.assign(suggestion.url);
  });

  /* 
    If no hits in the Autocomplete dropdown are highlighted,
    treat input like normal search bar
  */
  const searchForm = document.getElementById('search-form');
  const input = document.getElementById('search-input');
  let searchQuery, hitSelected, hits;

  input.addEventListener('keyup', e => {
    searchQuery = input.value;
  });

  /*
    Prevent form from being submitted when magnifying
    glass is clicked or enter pressed with no query
    or hits
  */
  searchForm.addEventListener('submit', e => {
    e.preventDefault();
  });

  /*
    Search for highlighted hit or search query
    when search button or enter is pressed
  */
  function submitSearch() {
    hitSelected = document.getElementsByClassName('aa-cursor')[0];

    if (hitSelected && searchQuery) {
      const articleUrl = hitSelected.querySelector('a').href;
      window.location.assign(articleUrl);
    } else if (!hitSelected && searchQuery && hits) {
      window.location.assign(`https://www.freecodecamp.org/news/search?query=${searchQuery}`);
    }
  }
</script>
    </div>
    <div class="site-nav-middle">
        <a class="site-nav-logo" href="https://www.freecodecamp.org/news"><img src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/fcc_primary_large_24X210.svg" alt="freeCodeCamp.org"></a>
    </div>
    <div class="site-nav-right">
        <a class="toggle-button-nav" href="https://www.freecodecamp.org/donate/">
            Donate
        </a>
    </div>

</nav>
        <div class="under-header-content jumbotron">
    <h2 class="donation-banner">
        Stay safe, friends. Learn to code from home. <a href="https://www.freecodecamp.org/">Use our free 2,000 hour
            curriculum.</a>
    </h2>
</div>
        <div id="error-message"></div>

        




<main id="site-main" class="site-main outer">
    <div class="inner">

        <article class="post-full post tag-machine-learning tag-python ">

            <header class="post-full-header">
                <section class="post-full-meta">
                    <time class="post-full-meta-date" datetime="2020-07-03">3 July 2020</time>
                    <span class="date-divider">/</span>
                    <a href="https://www.freecodecamp.org/news/tag/machine-learning/">
                        #Machine Learning
                    </a>
                </section>
                <h1 class="post-full-title">How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python</h1>
            </header>

            <div class="post-full-author-header">


                
<section class="author-card">
    <img class="author-profile-image" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/0Y2A0586-2.jpg" alt="Nick McCullum">
    <section class="author-card-content">
        <h4 class="author-card-name"><a href="https://www.freecodecamp.org/news/author/nick/">Nick McCullum</a></h4>
        <p>I write about software, machine learning, and entrepreneurship at https://nickmccullum.com. I also sell premium courses on Python programming and machine learning.</p>
    </section>
</section>


            </div>

            <figure class="post-full-image">
                <img srcset="/news/content/images/size/w300/2020/07/classificaton.png 300w,
                            /news/content/images/size/w600/2020/07/classificaton.png 600w,
                            /news/content/images/size/w1000/2020/07/classificaton.png 1000w,
                            /news/content/images/size/w2000/2020/07/classificaton.png 2000w" sizes="(max-width: 800px) 400px,
                            (max-width: 1170px) 700px,
                            1400px" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/classificaton.png" alt="How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python" onerror="this.style.display=&#39;none&#39;">
            </figure>

            <section class=" post-full-content">
                <div class="post-content">
                    <p>One of <a href="https://gumroad.com/l/pGjwd">machine learning's most popular applications</a> is in solving classification problems.</p><p>Classification problems are situations where you have a data set, and you want to classify observations from that data set into a specific category. </p><p>A famous example is a spam filter for email providers. Gmail uses supervised machine learning techniques to automatically place emails in your spam folder based on their content, subject line, and other features.</p><p>Two machine learning models perform much of the heavy lifting when it comes to classification problems:</p><ul><li>K-nearest neighbors</li><li>K-means clustering</li></ul><p>This tutorial will teach you how to code K-nearest neighbors and K-means clustering algorithms in Python.</p><h1 id="k-nearest-neighbors-models">K-Nearest Neighbors Models</h1><p>The <a href="https://nickmccullum.com/python-machine-learning/k-nearest-neighbors-python/">K-nearest neighbors algorithm</a> is one of the world’s most popular machine learning models for solving classification problems.</p><p>A common exercise for students exploring machine learning is to apply the K nearest neighbors algorithm to a data set where the categories are not known. A real-life example of this would be if you needed to make predictions using machine learning on a data set of classified government information.</p><p>In this tutorial, you will learn to write your first K nearest neighbors machine learning algorithm in Python. We will be working with an anonymous data set similar to the situation described above.</p><h2 id="the-data-set-you-will-need-in-this-tutorial"><strong>The Data Set You Will Need in This Tutorial</strong></h2><p>The first thing you need to do is download the data set we will be using in this tutorial. I have uploaded the file to <a href="https://nickmccullum.com/">my website</a>. You can access it by clicking <a href="https://nickmccullum.com/files/k-nearest-neighbors/classified_data.csv">here</a>.</p><p>Now that you have downloaded the data set, you will want to move the file to the directory that you’ll be working in. After that, open a <a href="https://nickmccullum.com/python-course/jupyter-notebook-basics/">Jupyter Notebook</a> and we can get started writing Python code!</p><h2 id="the-libraries-you-will-need-in-this-tutorial"><strong>The Libraries You Will Need in This Tutorial</strong></h2><p>To write a K nearest neighbors algorithm, we will take advantage of many open-source Python libraries including <a href="https://nickmccullum.com/advanced-python/numpy/">NumPy</a>, <a href="https://nickmccullum.com/advanced-python/pandas-dataframes/">pandas</a>, and <a href="https://nickmccullum.com/python-machine-learning/introduction-scikit-learn/">scikit-learn</a>.</p><p>Begin your Python script by writing the following import statements:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">import</span> numpy <span class="token keyword">as</span> np

<span class="token keyword">import</span> pandas <span class="token keyword">as</span> pd

<span class="token keyword">import</span> matplotlib<span class="token punctuation">.</span>pyplot <span class="token keyword">as</span> plt

<span class="token keyword">import</span> seaborn <span class="token keyword">as</span> sns

<span class="token operator">%</span>matplotlib inline

</code></pre><!--kg-card-end: code--><h2 id="importing-the-data-set-into-our-python-script"><strong>Importing the Data Set Into Our Python Script</strong></h2><p>Our next step is to import the <code>classified_data.csv</code> file into our Python script. The pandas library makes it easy to<a href="https://nickmccullum.com/advanced-python/pandas-data-input-output/"> import data into a pandas DataFrame</a>.</p><p>Since the data set is stored in a <code>csv</code> file, we will be using the <code>read_csv</code> method to do this:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
raw_data <span class="token operator">=</span> pd<span class="token punctuation">.</span>read_csv<span class="token punctuation">(</span><span class="token string">'classified_data.csv'</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Printing this DataFrame inside of your Jupyter Notebook will give you a sense of what the data looks like:</p><!--kg-card-begin: image--><figure class="kg-card kg-image-card"><img src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/pandas-dataframe.png" class="kg-image" alt="A pandas DataFrame"></figure><!--kg-card-end: image--><p>You will notice that the DataFrame starts with an unnamed column whose values are equal to the DataFrame’s index. We can fix this by making a slight adjustment to the command that imported our data set into the Python script:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
raw_data <span class="token operator">=</span> pd<span class="token punctuation">.</span>read_csv<span class="token punctuation">(</span><span class="token string">'classified_data.csv'</span><span class="token punctuation">,</span> index_col <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Next, let’s take a look at the actual features that are contained in this data set. You can print a list of the data set’s column names with the following statement:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">print</span><span class="token punctuation">(</span>raw_data<span class="token punctuation">.</span>columns<span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>This returns:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
Index<span class="token punctuation">(</span><span class="token punctuation">[</span><span class="token string">'WTT'</span><span class="token punctuation">,</span> <span class="token string">'PTI'</span><span class="token punctuation">,</span> <span class="token string">'EQW'</span><span class="token punctuation">,</span> <span class="token string">'SBI'</span><span class="token punctuation">,</span> <span class="token string">'LQE'</span><span class="token punctuation">,</span> <span class="token string">'QWG'</span><span class="token punctuation">,</span> <span class="token string">'FDJ'</span><span class="token punctuation">,</span> <span class="token string">'PJF'</span><span class="token punctuation">,</span> <span class="token string">'HQE'</span><span class="token punctuation">,</span> <span class="token string">'NXJ'</span><span class="token punctuation">,</span>

       <span class="token string">'TARGET CLASS'</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

      dtype<span class="token operator">=</span><span class="token string">'object'</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Since this is a classified data set, we have no idea what any of these columns means. For now, it is sufficient to recognize that every column is numerical in nature and thus well-suited for modelling with machine learning techniques.</p><h2 id="standardizing-the-data-set"><strong>Standardizing the Data Set</strong></h2><p>Since the K nearest neighbors algorithm makes predictions about a data point by using the observations that are closest to it, the scale of the features within a data set matters a lot.</p><p>Because of this, machine learning practitioners typically <code>standardize</code> the data set, which means adjusting every <code>x</code> value so that they are roughly on the same scale.</p><p>Fortunately, <code>scikit-learn</code> includes some excellent functionality to do this with very little headache.</p><p>To start, we will need to import the <code>StandardScaler</code> class from <code>scikit-learn</code>. Add the following command to your Python script to do this:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>preprocessing <span class="token keyword">import</span> StandardScaler

</code></pre><!--kg-card-end: code--><p>This function behaves a lot like the <code>LinearRegression</code> and <code>LogisticRegression</code> classes that we used earlier in this course. We will want to create an instance of this class and then fit the instance of that class on our data set.</p><p>First, let’s create an instance of the <code>StandardScaler</code> class named <code>scaler</code> with the following statement:</p><!--kg-card-begin: code--><pre><code>
scaler = StandardScaler()

</code></pre><!--kg-card-end: code--><p>We can now train this instance on our data set using the <code>fit</code> method:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
scaler<span class="token punctuation">.</span>fit<span class="token punctuation">(</span>raw_data<span class="token punctuation">.</span>drop<span class="token punctuation">(</span><span class="token string">'TARGET CLASS'</span><span class="token punctuation">,</span> axis<span class="token operator">=</span><span class="token number">1</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Now we can use the <code>transform</code> method to standardize all of the features in the data set so they are roughly the same scale. We’ll assign these scaled features to the variable named <code>scaled_features</code>:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
scaled_features <span class="token operator">=</span> scaler<span class="token punctuation">.</span>transform<span class="token punctuation">(</span>raw_data<span class="token punctuation">.</span>drop<span class="token punctuation">(</span><span class="token string">'TARGET CLASS'</span><span class="token punctuation">,</span> axis<span class="token operator">=</span><span class="token number">1</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>This actually creates a <a href="https://nickmccullum.com/advanced-python/numpy-arrays/">NumPy array</a> of all the features in the data set, and we want it to be a <a href="https://nickmccullum.com/advanced-python/pandas-dataframes/">pandas DataFrame</a> instead.</p><p>Fortunately, this is an easy fix. We’ll simply wrap the <code>scaled_features</code> variable in a <code>pd.DataFrame</code> method and assign this DataFrame to a new variable called <code>scaled_data</code> with an appropriate argument to specify the column names:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
scaled_data <span class="token operator">=</span> pd<span class="token punctuation">.</span>DataFrame<span class="token punctuation">(</span>scaled_features<span class="token punctuation">,</span> columns <span class="token operator">=</span> raw_data<span class="token punctuation">.</span>drop<span class="token punctuation">(</span><span class="token string">'TARGET CLASS'</span><span class="token punctuation">,</span> axis<span class="token operator">=</span><span class="token number">1</span><span class="token punctuation">)</span><span class="token punctuation">.</span>columns<span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Now that we have imported our data set and standardized its features, we are ready to split the data set into training data and test data.</p><h2 id="splitting-the-data-set-into-training-data-and-test-data"><strong>Splitting the Data Set Into Training Data and Test Data</strong></h2><p>We will use the <code>train_test_split</code> function from <code>scikit-learn</code> combined with list unpacking to create training data and test data from our classified data set.</p><p>First, you’ll need to import <code>train_test_split</code> from the <code>model_validation</code> module of <code>scikit-learn</code> with the following statement:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>model_selection <span class="token keyword">import</span> train_test_split

</code></pre><!--kg-card-end: code--><p>Next, we will need to specify the <code>x</code> and <code>y</code> values that will be passed into this <code>train_test_split</code> function.</p><p>The <code>x</code> values will be the <code>scaled_data</code> DataFrame that we created previously. The <code>y</code> values will be the <code>TARGET CLASS</code> column of our original <code>raw_data</code> DataFrame.</p><p>You can create these variables with the following statements:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
x <span class="token operator">=</span> scaled_data

y <span class="token operator">=</span> raw_data<span class="token punctuation">[</span><span class="token string">'TARGET CLASS'</span><span class="token punctuation">]</span>

</code></pre><!--kg-card-end: code--><p>Next, you’ll need to run the <code>train_test_split</code> function using these two arguments and a reasonable <code>test_size</code>. We will use a <code>test_size</code> of 30%, which gives the following parameters for the function:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
x_training_data<span class="token punctuation">,</span> x_test_data<span class="token punctuation">,</span> y_training_data<span class="token punctuation">,</span> y_test_data <span class="token operator">=</span> train_test_split<span class="token punctuation">(</span>x<span class="token punctuation">,</span> y<span class="token punctuation">,</span> test_size <span class="token operator">=</span> <span class="token number">0.3</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Now that our data set has been split into training data and test data, we’re ready to start training our model!</p><h2 id="training-a-k-nearest-neighbors-model"><strong>Training a K Nearest Neighbors Model</strong></h2><p>Let’s start by importing the <code>KNeighborsClassifier</code> from <code>scikit-learn</code>:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>neighbors <span class="token keyword">import</span> KNeighborsClassifier

</code></pre><!--kg-card-end: code--><p>Next, let’s create an instance of the <code>KNeighborsClassifier</code> class and assign it to a variable named <code>model</code></p><p>This class requires a parameter named <code>n_neighbors</code>, which is equal to the <code>K</code> value of the K nearest neighbors algorithm that you’re building. To start, let’s specify <code>n_neighbors = 1</code>:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
model <span class="token operator">=</span> KNeighborsClassifier<span class="token punctuation">(</span>n_neighbors <span class="token operator">=</span> <span class="token number">1</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Now we can train our K nearest neighbors model using the <code>fit</code> method and our <code>x_training_data</code> and <code>y_training_data</code> variables:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
model<span class="token punctuation">.</span>fit<span class="token punctuation">(</span>x_training_data<span class="token punctuation">,</span> y_training_data<span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Now let’s make some predictions with our newly-trained K nearest neighbors algorithm!</p><h2 id="making-predictions-with-our-k-nearest-neighbors-algorithm"><strong>Making Predictions With Our K Nearest Neighbors Algorithm</strong></h2><p>We can make predictions with our K nearest neighbors algorithm in the same way that we did with our <a href="https://nickmccullum.com/python-machine-learning/linear-regression-python/">linear regression</a> and <a href="https://nickmccullum.com/python-machine-learning/logistic-regression-python/">logistic regression</a> models earlier in this course: by using the <code>predict</code> method and passing in our <code>x_test_data</code> variable.</p><p>More specifically, here’s how you can make predictions and assign them to a variable called <code>predictions</code>:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
predictions <span class="token operator">=</span> model<span class="token punctuation">.</span>predict<span class="token punctuation">(</span>x_test_data<span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Let’s explore how accurate our <code>predictions</code> are in the next section of this tutorial.</p><h2 id="measuring-the-accuracy-of-our-model"><strong>Measuring the Accuracy of Our Model</strong></h2><p>We saw in our logistic regression tutorial that <code>scikit-learn</code> comes with built-in functions that make it easy to measure the performance of machine learning classification models.</p><p>Let’s import two of these functions (<code>classification_report</code> and <code>confuson_matrix</code>) into our report now:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>metrics <span class="token keyword">import</span> classification_report

<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>metrics <span class="token keyword">import</span> confusion_matrix

</code></pre><!--kg-card-end: code--><p>Let’s work through each of these one-by-one, starting with the <code>classfication_report</code>. You can generate the report with the following statement:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">print</span><span class="token punctuation">(</span>classification_report<span class="token punctuation">(</span>y_test_data<span class="token punctuation">,</span> predictions<span class="token punctuation">)</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>This generates:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
             precision    recall  f1<span class="token operator">-</span>score   support

           <span class="token number">0</span>       <span class="token number">0.94</span>      <span class="token number">0.85</span>      <span class="token number">0.89</span>       <span class="token number">150</span>

           <span class="token number">1</span>       <span class="token number">0.86</span>      <span class="token number">0.95</span>      <span class="token number">0.90</span>       <span class="token number">150</span>

    accuracy                           <span class="token number">0.90</span>       <span class="token number">300</span>

   macro avg       <span class="token number">0.90</span>      <span class="token number">0.90</span>      <span class="token number">0.90</span>       <span class="token number">300</span>

weighted avg       <span class="token number">0.90</span>      <span class="token number">0.90</span>      <span class="token number">0.90</span>       <span class="token number">300</span>

</code></pre><!--kg-card-end: code--><p>Similarly, you can generate a confusion matrix with the following statement:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">print</span><span class="token punctuation">(</span>confusion_matrix<span class="token punctuation">(</span>y_test_data<span class="token punctuation">,</span> predictions<span class="token punctuation">)</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>This generates:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token punctuation">[</span><span class="token punctuation">[</span><span class="token number">141</span>  <span class="token number">12</span><span class="token punctuation">]</span>

 <span class="token punctuation">[</span> <span class="token number">18</span> <span class="token number">129</span><span class="token punctuation">]</span><span class="token punctuation">]</span>

</code></pre><!--kg-card-end: code--><p>Looking at these performance metrics, it looks like our model is already fairly performant. It can still be improved.</p><p>In the next section, we will see how we can improve the performance of our K nearest neighbors model by choosing a better value for <code>K</code>.</p><h2 id="choosing-an-optimal-k-value-using-the-elbow-method"><strong>Choosing An Optimal <code>K</code> Value Using the Elbow Method</strong></h2><p>In this section, we will use the elbow method to choose an optimal value of <code>K</code> for our K nearest neighbors algorithm.</p><p>The elbow method involves iterating through different K values and selecting the value with the lowest error rate when applied to our test data.</p><p>To start, let’s create an empty <a href="https://nickmccullum.com/python-course/lists/">list</a> called <code>error_rates</code>. We will loop through different <code>K</code> values and append their error rates to this list.</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
error_rates <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>

</code></pre><!--kg-card-end: code--><p>Next, we need to make a Python loop that iterates through the different values of <code>K</code> we’d like to test and executes the following functionality with each iteration:</p><ul><li>Creates a new instance of the <code>KNeighborsClassifier</code> class from <code>scikit-learn</code></li><li>Trains the new model using our training data</li><li>Makes predictions on our test data</li><li>Calculates the mean difference for every incorrect prediction (the lower this is, the more accurate our model is)</li></ul><p>Here is the code to do this for <code>K</code> values between <code>1</code> and <code>100</code>:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">for</span> i <span class="token keyword">in</span> np<span class="token punctuation">.</span>arange<span class="token punctuation">(</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">101</span><span class="token punctuation">)</span><span class="token punctuation">:</span>

    new_model <span class="token operator">=</span> KNeighborsClassifier<span class="token punctuation">(</span>n_neighbors <span class="token operator">=</span> i<span class="token punctuation">)</span>

    new_model<span class="token punctuation">.</span>fit<span class="token punctuation">(</span>x_training_data<span class="token punctuation">,</span> y_training_data<span class="token punctuation">)</span>

    new_predictions <span class="token operator">=</span> new_model<span class="token punctuation">.</span>predict<span class="token punctuation">(</span>x_test_data<span class="token punctuation">)</span>

    error_rates<span class="token punctuation">.</span>append<span class="token punctuation">(</span>np<span class="token punctuation">.</span>mean<span class="token punctuation">(</span>new_predictions <span class="token operator">!=</span> y_test_data<span class="token punctuation">)</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Let’s visualize how our error rate changes with different <code>K</code> values using a quick matplotlib visualization:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
plt<span class="token punctuation">.</span>plot<span class="token punctuation">(</span>error_rates<span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><!--kg-card-begin: image--><figure class="kg-card kg-image-card"><img src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/error-rates.png" class="kg-image" alt="A plot of our error rates"></figure><!--kg-card-end: image--><p>As you can see, our error rates tend to be minimized with a <code>K</code> value of approximately 50. This means that <code>50</code> is a suitable choice for <code>K</code> that balances both simplicity and predictive power.</p><h2 id="the-full-code-for-this-tutorial"><strong>The Full Code For This Tutorial</strong></h2><p>You can view the full code for this tutorial in <a href="https://github.com/nicholasmccullum/python-machine-learning">this GitHub repository</a>. It is also pasted below for your reference:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token comment">#Common imports</span>

<span class="token keyword">import</span> numpy <span class="token keyword">as</span> np

<span class="token keyword">import</span> pandas <span class="token keyword">as</span> pd

<span class="token keyword">import</span> matplotlib<span class="token punctuation">.</span>pyplot <span class="token keyword">as</span> plt

<span class="token keyword">import</span> seaborn <span class="token keyword">as</span> sns

<span class="token operator">%</span>matplotlib inline

<span class="token comment">#Import the data set</span>

raw_data <span class="token operator">=</span> pd<span class="token punctuation">.</span>read_csv<span class="token punctuation">(</span><span class="token string">'classified_data.csv'</span><span class="token punctuation">,</span> index_col <span class="token operator">=</span> <span class="token number">0</span><span class="token punctuation">)</span>

<span class="token comment">#Import standardization functions from scikit-learn</span>

<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>preprocessing <span class="token keyword">import</span> StandardScaler

<span class="token comment">#Standardize the data set</span>

scaler <span class="token operator">=</span> StandardScaler<span class="token punctuation">(</span><span class="token punctuation">)</span>

scaler<span class="token punctuation">.</span>fit<span class="token punctuation">(</span>raw_data<span class="token punctuation">.</span>drop<span class="token punctuation">(</span><span class="token string">'TARGET CLASS'</span><span class="token punctuation">,</span> axis<span class="token operator">=</span><span class="token number">1</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

scaled_features <span class="token operator">=</span> scaler<span class="token punctuation">.</span>transform<span class="token punctuation">(</span>raw_data<span class="token punctuation">.</span>drop<span class="token punctuation">(</span><span class="token string">'TARGET CLASS'</span><span class="token punctuation">,</span> axis<span class="token operator">=</span><span class="token number">1</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

scaled_data <span class="token operator">=</span> pd<span class="token punctuation">.</span>DataFrame<span class="token punctuation">(</span>scaled_features<span class="token punctuation">,</span> columns <span class="token operator">=</span> raw_data<span class="token punctuation">.</span>drop<span class="token punctuation">(</span><span class="token string">'TARGET CLASS'</span><span class="token punctuation">,</span> axis<span class="token operator">=</span><span class="token number">1</span><span class="token punctuation">)</span><span class="token punctuation">.</span>columns<span class="token punctuation">)</span>

<span class="token comment">#Split the data set into training data and test data</span>

<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>model_selection <span class="token keyword">import</span> train_test_split

x <span class="token operator">=</span> scaled_data

y <span class="token operator">=</span> raw_data<span class="token punctuation">[</span><span class="token string">'TARGET CLASS'</span><span class="token punctuation">]</span>

x_training_data<span class="token punctuation">,</span> x_test_data<span class="token punctuation">,</span> y_training_data<span class="token punctuation">,</span> y_test_data <span class="token operator">=</span> train_test_split<span class="token punctuation">(</span>x<span class="token punctuation">,</span> y<span class="token punctuation">,</span> test_size <span class="token operator">=</span> <span class="token number">0.3</span><span class="token punctuation">)</span>

<span class="token comment">#Train the model and make predictions</span>

<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>neighbors <span class="token keyword">import</span> KNeighborsClassifier

model <span class="token operator">=</span> KNeighborsClassifier<span class="token punctuation">(</span>n_neighbors <span class="token operator">=</span> <span class="token number">1</span><span class="token punctuation">)</span>

model<span class="token punctuation">.</span>fit<span class="token punctuation">(</span>x_training_data<span class="token punctuation">,</span> y_training_data<span class="token punctuation">)</span>

predictions <span class="token operator">=</span> model<span class="token punctuation">.</span>predict<span class="token punctuation">(</span>x_test_data<span class="token punctuation">)</span>

<span class="token comment">#Performance measurement</span>

<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>metrics <span class="token keyword">import</span> classification_report

<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>metrics <span class="token keyword">import</span> confusion_matrix

<span class="token keyword">print</span><span class="token punctuation">(</span>classification_report<span class="token punctuation">(</span>y_test_data<span class="token punctuation">,</span> predictions<span class="token punctuation">)</span><span class="token punctuation">)</span>

<span class="token keyword">print</span><span class="token punctuation">(</span>confusion_matrix<span class="token punctuation">(</span>y_test_data<span class="token punctuation">,</span> predictions<span class="token punctuation">)</span><span class="token punctuation">)</span>

<span class="token comment">#Selecting an optimal K value</span>

error_rates <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token punctuation">]</span>

<span class="token keyword">for</span> i <span class="token keyword">in</span> np<span class="token punctuation">.</span>arange<span class="token punctuation">(</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">101</span><span class="token punctuation">)</span><span class="token punctuation">:</span>

    new_model <span class="token operator">=</span> KNeighborsClassifier<span class="token punctuation">(</span>n_neighbors <span class="token operator">=</span> i<span class="token punctuation">)</span>

    new_model<span class="token punctuation">.</span>fit<span class="token punctuation">(</span>x_training_data<span class="token punctuation">,</span> y_training_data<span class="token punctuation">)</span>

    new_predictions <span class="token operator">=</span> new_model<span class="token punctuation">.</span>predict<span class="token punctuation">(</span>x_test_data<span class="token punctuation">)</span>

    error_rates<span class="token punctuation">.</span>append<span class="token punctuation">(</span>np<span class="token punctuation">.</span>mean<span class="token punctuation">(</span>new_predictions <span class="token operator">!=</span> y_test_data<span class="token punctuation">)</span><span class="token punctuation">)</span>

plt<span class="token punctuation">.</span>figure<span class="token punctuation">(</span>figsize<span class="token operator">=</span><span class="token punctuation">(</span><span class="token number">16</span><span class="token punctuation">,</span><span class="token number">12</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

plt<span class="token punctuation">.</span>plot<span class="token punctuation">(</span>error_rates<span class="token punctuation">)</span>
</code></pre><!--kg-card-end: code--><h1 id="k-means-clustering-models">K-Means Clustering Models</h1><p>The <a href="https://nickmccullum.com/python-machine-learning/k-means-clustering-python/">K-means clustering algorithm</a> is typically the first unsupervised machine learning model that students will learn.</p><p>It allows machine learning practitioners to create groups of data points within a data set with similar quantitative characteristics. It is useful for solving problems like creating customer segments or identifying localities in a city with high crime rates.</p><p>In this section, you will learn how to build your first K means clustering algorithm in Python.</p><h2 id="the-data-set-we-will-use-in-this-tutorial"><strong>The Data Set We Will Use In This Tutorial</strong></h2><p>In this tutorial, we will be using a data set of data generated using <code>scikit-learn</code>.</p><p>Let’s import <code>scikit-learn</code>’s <code>make_blobs</code> function to create this artificial data. Open up a <a href="https://nickmccullum.com/python-course/jupyter-notebook-basics/">Jupyter Notebook</a> and start your Python script with the following statement:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>datasets <span class="token keyword">import</span> make_blobs

</code></pre><!--kg-card-end: code--><p>Now let’s use the <code>make_blobs</code> function to create some artificial data!</p><p>More specifically, here is how you could create a data set with <code>200</code> samples that has <code>2</code> features and <code>4</code> cluster centers. The standard deviation within each cluster will be set to <code>1.8</code>.</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
raw_data <span class="token operator">=</span> make_blobs<span class="token punctuation">(</span>n_samples <span class="token operator">=</span> <span class="token number">200</span><span class="token punctuation">,</span> n_features <span class="token operator">=</span> <span class="token number">2</span><span class="token punctuation">,</span> centers <span class="token operator">=</span> <span class="token number">4</span><span class="token punctuation">,</span> cluster_std <span class="token operator">=</span> <span class="token number">1.8</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>If you print this <code>raw_data</code> object, you’ll notice that it is actually a <a href="https://nickmccullum.com/python-course/tuples/">Python tuple</a>. The first element of this tuple is a <a href="https://nickmccullum.com/advanced-python/numpy-arrays/">NumPy array</a> with 200 observations. Each observation contains 2 features (just like we specified with our <code>make_blobs</code> function!).</p><p>Now that our data has been created, we can move on to importing other important open-source libraries into our Python script.</p><h2 id="the-imports-we-will-use-in-this-tutorial"><strong>The Imports We Will Use In This Tutorial</strong></h2><p>This tutorial will make use of a number of popular open-source Python libraries, including <a href="https://nickmccullum.com/advanced-python/pandas/">pandas</a>, <a href="https://nickmccullum.com/advanced-python/numpy/">NumPy</a>, and <a href="https://nickmccullum.com/python-visualization/how-to-import-matplotlib/">matplotlib</a>. Let’s continue our Python script by adding the following imports:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">import</span> pandas <span class="token keyword">as</span> pd

<span class="token keyword">import</span> numpy <span class="token keyword">as</span> np

<span class="token keyword">import</span> seaborn

<span class="token keyword">import</span> matplotlib<span class="token punctuation">.</span>pyplot <span class="token keyword">as</span> plt

<span class="token operator">%</span>matplotlib inline

</code></pre><!--kg-card-end: code--><p>The first group of imports in this code block is for manipulating large data sets. The second group of imports is for creating data visualizations.</p><p>Let’s move on to visualizing our data set next.</p><h2 id="visualizing-our-data-set"><strong>Visualizing Our Data Set</strong></h2><p>In our <code>make_blobs</code> function, we specified for our data set to have 4 cluster centers. The best way to verify that this has been handled correctly is by creating some quick data visualizations.</p><p>To start, let’s use the following command to plot all of the rows in the first column of our data set against all of the rows in the second column of our data set:</p><!--kg-card-begin: image--><figure class="kg-card kg-image-card"><img src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/first-scatterplot.png" class="kg-image" alt="A scatterplot of our artificial data"></figure><!--kg-card-end: image--><p><em><em>Note: your data set will appear differently than mine since this is randomly-generated data.</em></em></p><p>This image seems to indicate that our data set has only three clusters. This is because two of the clusters are very close to each other.</p><p>To fix this, we need to reference the second element of our <code>raw_data</code> tuple, which is a NumPy array that contains the cluster to which each observation belongs.</p><p>If we color our data set using each observation’s cluster, the unique clusters will quickly become clear. Here is the code to do this:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
plt<span class="token punctuation">.</span>scatter<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">,</span> raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">,</span> c<span class="token operator">=</span>raw_data<span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><!--kg-card-begin: image--><figure class="kg-card kg-image-card"><img src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/second-scatterplot.png" class="kg-image" alt="A scatterplot of our artificial data"></figure><!--kg-card-end: image--><p>We can now see that our data set has four unique clusters. Let’s move on to building our K means cluster model in Python!</p><h2 id="building-and-training-our-k-means-clustering-model"><strong>Building and Training Our K Means Clustering Model</strong></h2><p>The first step to building our K means clustering algorithm is importing it from <code>scikit-learn</code>. To do this, add the following command to your Python script:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>cluster <span class="token keyword">import</span> KMeans

</code></pre><!--kg-card-end: code--><p>Next, lets create an instance of this <code>KMeans</code> class with a parameter of <code>n_clusters=4</code> and assign it to the variable <code>model</code>:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
model <span class="token operator">=</span> KMeans<span class="token punctuation">(</span>n_clusters<span class="token operator">=</span><span class="token number">4</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>Now let’s train our model by invoking the <code>fit</code> method on it and passing in the first element of our <code>raw_data</code> tuple:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
model<span class="token punctuation">.</span>fit<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>In the next section, we’ll explore how to make predictions with this K means clustering model.</p><p>Before moving on, I wanted to point out one difference that you may have noticed between the process for building this K means clustering algorithm (which is an unsupervised machine learning algorithm) and the supervised machine learning algorithms we’ve worked with so far in this course.</p><p>Namely, we did not have to split the data set into training data and test data. This is an important difference - and in fact, you never need to make the train/test split on a data set when building unsupervised machine learning models!</p><h2 id="making-predictions-with-our-k-means-clustering-model"><strong>Making Predictions With Our K Means Clustering Model</strong></h2><p>Machine learning practitioners generally use K means clustering algorithms to make two types of predictions:</p><ul><li>Which cluster each data point belongs to</li><li>Where the center of each cluster is</li></ul><p>It is easy to generate these predictions now that our model has been trained.</p><p>First, let’s predict which cluster each data point belongs to. To do this, access the <code>labels_</code> attribute from our <code>model</code> object using the dot operator, like this:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
model<span class="token punctuation">.</span>labels_

</code></pre><!--kg-card-end: code--><p>This generates a NumPy array with predictions for each data point that looks like this:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
array<span class="token punctuation">(</span><span class="token punctuation">[</span><span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span>

       <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span>

       <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span>

       <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span>

       <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span>

       <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span>

       <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span>

       <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span>

       <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">7</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span> <span class="token number">5</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> <span class="token number">4</span><span class="token punctuation">,</span> <span class="token number">6</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">,</span>

       <span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">,</span> dtype<span class="token operator">=</span>int32<span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>To see where the center of each cluster lies, access the <code>cluster_centers_</code> attribute using the dot operator like this:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
model<span class="token punctuation">.</span>cluster_centers_

</code></pre><!--kg-card-end: code--><p>This generates a two-dimensional NumPy array that contains the coordinates of each clusters center. It will look like this:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
array<span class="token punctuation">(</span><span class="token punctuation">[</span><span class="token punctuation">[</span> <span class="token operator">-</span><span class="token number">8.06473328</span><span class="token punctuation">,</span>  <span class="token operator">-</span><span class="token number">0.42044783</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

       <span class="token punctuation">[</span>  <span class="token number">0.15944397</span><span class="token punctuation">,</span>  <span class="token operator">-</span><span class="token number">9.4873621</span> <span class="token punctuation">]</span><span class="token punctuation">,</span>

       <span class="token punctuation">[</span>  <span class="token number">1.49194628</span><span class="token punctuation">,</span>   <span class="token number">0.21216413</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

       <span class="token punctuation">[</span><span class="token operator">-</span><span class="token number">10.97238157</span><span class="token punctuation">,</span>  <span class="token operator">-</span><span class="token number">2.49017206</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

       <span class="token punctuation">[</span>  <span class="token number">3.54673215</span><span class="token punctuation">,</span>  <span class="token operator">-</span><span class="token number">9.7433692</span> <span class="token punctuation">]</span><span class="token punctuation">,</span>

       <span class="token punctuation">[</span> <span class="token operator">-</span><span class="token number">3.41262049</span><span class="token punctuation">,</span>   <span class="token number">7.80784834</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

       <span class="token punctuation">[</span>  <span class="token number">2.53980034</span><span class="token punctuation">,</span>  <span class="token operator">-</span><span class="token number">2.96376999</span><span class="token punctuation">]</span><span class="token punctuation">,</span>

       <span class="token punctuation">[</span> <span class="token operator">-</span><span class="token number">0.4195847</span> <span class="token punctuation">,</span>   <span class="token number">6.92561289</span><span class="token punctuation">]</span><span class="token punctuation">]</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>We’ll assess the accuracy of these predictions in the next section.</p><h2 id="visualizing-the-accuracy-of-our-model"><strong>Visualizing the Accuracy of Our Model</strong></h2><p>The last thing we’ll do in this tutorial is visualize the accuracy of our model. You can use the following code to do this:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
f<span class="token punctuation">,</span> <span class="token punctuation">(</span>ax1<span class="token punctuation">,</span> ax2<span class="token punctuation">)</span> <span class="token operator">=</span> plt<span class="token punctuation">.</span>subplots<span class="token punctuation">(</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> sharey<span class="token operator">=</span><span class="token boolean">True</span><span class="token punctuation">,</span>figsize<span class="token operator">=</span><span class="token punctuation">(</span><span class="token number">10</span><span class="token punctuation">,</span><span class="token number">6</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

ax1<span class="token punctuation">.</span>set_title<span class="token punctuation">(</span><span class="token string">'Our Model'</span><span class="token punctuation">)</span>

ax1<span class="token punctuation">.</span>scatter<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">,</span> raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">,</span>c<span class="token operator">=</span>model<span class="token punctuation">.</span>labels_<span class="token punctuation">)</span>

ax2<span class="token punctuation">.</span>set_title<span class="token punctuation">(</span><span class="token string">'Original Data'</span><span class="token punctuation">)</span>

ax2<span class="token punctuation">.</span>scatter<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">,</span> raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">,</span>c<span class="token operator">=</span>raw_data<span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">)</span>

</code></pre><!--kg-card-end: code--><p>This generates two different plots side-by-side where one plot shows the clusters according to the real data set and the other plot shows the clusters according to our model. Here is what the output looks like:</p><!--kg-card-begin: image--><figure class="kg-card kg-image-card"><img src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/k-means-clustering-subplots.png" class="kg-image" alt="A scatterplot of our model&#39;s predictions"></figure><!--kg-card-end: image--><p>Although the coloring between the two plots is different, you can see that our model did a fairly good job of predicting the clusters within our data set. You can also see that the model was not perfect - if you look at the data points along a cluster’s edge, you can see that it occasionally misclassified an observation from our data set.</p><p>There’s one last thing that needs to be mentioned about measuring our model’s prediction. In this example ,we knew which cluster each observation belonged to because we actually generated this data set ourselves.</p><p>This is highly unusual. K means clustering is more often applied when the clusters aren’t known in advance. Instead, machine learning practitioners use K means clustering to find patterns that they don’t already know within a data set.</p><h2 id="the-full-code-for-this-tutorial-1"><strong>The Full Code For This Tutorial</strong></h2><p>You can view the full code for this tutorial in <a href="https://github.com/nicholasmccullum/python-machine-learning">this GitHub repository</a>. It is also pasted below for your reference:</p><!--kg-card-begin: code--><pre class=" language-py"><code class=" language-py">
<span class="token comment">#Create artificial data set</span>

<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>datasets <span class="token keyword">import</span> make_blobs

raw_data <span class="token operator">=</span> make_blobs<span class="token punctuation">(</span>n_samples <span class="token operator">=</span> <span class="token number">200</span><span class="token punctuation">,</span> n_features <span class="token operator">=</span> <span class="token number">2</span><span class="token punctuation">,</span> centers <span class="token operator">=</span> <span class="token number">4</span><span class="token punctuation">,</span> cluster_std <span class="token operator">=</span> <span class="token number">1.8</span><span class="token punctuation">)</span>

<span class="token comment">#Data imports</span>

<span class="token keyword">import</span> pandas <span class="token keyword">as</span> pd

<span class="token keyword">import</span> numpy <span class="token keyword">as</span> np

<span class="token comment">#Visualization imports</span>

<span class="token keyword">import</span> seaborn

<span class="token keyword">import</span> matplotlib<span class="token punctuation">.</span>pyplot <span class="token keyword">as</span> plt

<span class="token operator">%</span>matplotlib inline

<span class="token comment">#Visualize the data</span>

plt<span class="token punctuation">.</span>scatter<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">,</span> raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">)</span>

plt<span class="token punctuation">.</span>scatter<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">,</span> raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">,</span> c<span class="token operator">=</span>raw_data<span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">)</span>

<span class="token comment">#Build and train the model</span>

<span class="token keyword">from</span> sklearn<span class="token punctuation">.</span>cluster <span class="token keyword">import</span> KMeans

model <span class="token operator">=</span> KMeans<span class="token punctuation">(</span>n_clusters<span class="token operator">=</span><span class="token number">4</span><span class="token punctuation">)</span>

model<span class="token punctuation">.</span>fit<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">)</span>

<span class="token comment">#See the predictions</span>

model<span class="token punctuation">.</span>labels_

model<span class="token punctuation">.</span>cluster_centers_

<span class="token comment">#PLot the predictions against the original data set</span>

f<span class="token punctuation">,</span> <span class="token punctuation">(</span>ax1<span class="token punctuation">,</span> ax2<span class="token punctuation">)</span> <span class="token operator">=</span> plt<span class="token punctuation">.</span>subplots<span class="token punctuation">(</span><span class="token number">1</span><span class="token punctuation">,</span> <span class="token number">2</span><span class="token punctuation">,</span> sharey<span class="token operator">=</span><span class="token boolean">True</span><span class="token punctuation">,</span>figsize<span class="token operator">=</span><span class="token punctuation">(</span><span class="token number">10</span><span class="token punctuation">,</span><span class="token number">6</span><span class="token punctuation">)</span><span class="token punctuation">)</span>

ax1<span class="token punctuation">.</span>set_title<span class="token punctuation">(</span><span class="token string">'Our Model'</span><span class="token punctuation">)</span>

ax1<span class="token punctuation">.</span>scatter<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">,</span> raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">,</span>c<span class="token operator">=</span>model<span class="token punctuation">.</span>labels_<span class="token punctuation">)</span>

ax2<span class="token punctuation">.</span>set_title<span class="token punctuation">(</span><span class="token string">'Original Data'</span><span class="token punctuation">)</span>

ax2<span class="token punctuation">.</span>scatter<span class="token punctuation">(</span>raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">,</span> raw_data<span class="token punctuation">[</span><span class="token number">0</span><span class="token punctuation">]</span><span class="token punctuation">[</span><span class="token punctuation">:</span><span class="token punctuation">,</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">,</span>c<span class="token operator">=</span>raw_data<span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">)</span>
</code></pre><!--kg-card-end: code--><h2 id="final-thoughts">Final Thoughts</h2><p>This tutorial taught you how to how to build K-nearest neighbors and K-means clustering machine learning models in Python.</p><p><strong>If you're interested in learning more about machine learning, my book <a href="https://gumroad.com/l/pGjwd">Pragmatic Machine Learning</a> will teach you practical machine learning techniques by building 9 real projects. The book launches August 3rd. You can preorder it for 50% off using the link below:</strong></p><!--kg-card-begin: bookmark--><figure class="kg-card kg-bookmark-card"><a class="kg-bookmark-container" href="https://gumroad.com/l/pGjwd"><div class="kg-bookmark-content"><div class="kg-bookmark-title">Pragmatic Machine Learning</div><div class="kg-bookmark-description">Machine learning is changing the world. But it’s always been hard to learn machine learning... until now. Pragmatic Machine Learning is a step-by-step guide that will teach you machine learning fundamentals through building 9 real-world projects. You’ll learn: Linear regression, Logistic regression,…</div><div class="kg-bookmark-metadata"><img class="kg-bookmark-icon" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/favicon.ico"><span class="kg-bookmark-author">Nick McCullum</span><span class="kg-bookmark-publisher">Gumroad</span></div></div><div class="kg-bookmark-thumbnail"><img src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/Screen_20Shot_202020-06-29_20at_208.49.04_20AM.png"></div></a></figure><!--kg-card-end: bookmark--><p>Here is a brief summary of what you learned about K-nearest neighbors models in Python:</p><ul><li>How classified data is a common tool used to teach students how to solve their first K nearest neighbor problems</li><li>Why it’s important to standardize your data set when building K nearest neighbor models</li><li>How to split your data set into training data and test data using the <code>train_test_split</code> function</li><li>How to train your first K nearest neighbors model and make predictions with it</li><li>How to measure the performance of a K nearest neighbors model</li><li>How to use the elbow method to select an optimal value of K in a K nearest neighbors model</li></ul><p>Similarly, here is a brief summary of what you learned about K-means clustering models in Python:</p><ul><li>How to create artificial data in <code>scikit-learn</code> using the <code>make_blobs</code> function</li><li>How to build and train a K means clustering model</li><li>That unsupervised machine learning techniques do not require you to split your data into training data and test data</li><li>How to build and train a K means clustering model using <code>scikit-learn</code></li><li>How to visualizes the performance of a K means clustering algorithm when you know the clusters in advance</li></ul>
                </div>
                <hr>
                <p class="social-row">

    If you read this far, tweet to the author to show them you care.
    <a class="cta-button" onclick="window.open(`https://twitter.com/intent/tweet?text=Thank%20you%20@NickJMcCullum%20for%20writing%20this%20helpful%20article%2e%0A%0AHow%20to%20Build%20and%20Train%20K-Nearest%20Neighbors%20and%20K-Means%20Clustering%20ML%20Models%20in%20Python%0A%0Ahttps%3A%2F%2Fwww.freecodecamp.org%2Fnews%2Fhow-to-build-and-train-k-nearest-neighbors-ml-models-in-python%2F`, &#39;share-twitter&#39;, &#39;width=550, height=235&#39;); return false;">Tweet
        a thanks</a>
</p>                
<div class="learn-cta-row">
    <p>
        Learn to code for free. freeCodeCamp's open source curriculum has helped more than 40,000 people get jobs as
        developers. <a class="cta-button" href="https://www.freecodecamp.org/learn">Get started</a>
    </p>
</div>            </section>



        </article>
    </div>
</main>




        <footer class="site-footer">
    <div class="footer-container">
        <div class="footer-top">
            <div class="footer-desc-col">
                <p>freeCodeCamp is a donor-supported tax-exempt 501(c)(3) nonprofit organization (United States Federal
                    Tax Identification Number: 82-0779546)
                </p>
                <p>
                    Our mission: to help people learn to code for free. We accomplish this by creating thousands of
                    videos, articles, and interactive coding lessons - all freely available to the public. We also have
                    thousands of freeCodeCamp study groups around the world.
                </p>
                <p>
                    Donations to freeCodeCamp go toward our education initiatives, and help pay for servers, services,
                    and staff.
                </p>
                <p class="footer-donation">
                    You can&nbsp;<a href="https://freecodecamp.org/donate" class="inline" rel="noopener noreferrer" target="_blank">make a tax-deductible donation here</a>.
                </p>
            </div>
            <div class="trending-guides">
                <div class="col-header">Trending Guides</div>
                <div class="trending-guides-row">
                    <div class="footer-col footer-col-1">
                        <a href="https://www.freecodecamp.org/news/javascript-closure-tutorial-with-js-closure-example-code/">JavaScript
                            Closure</a>
                        <a href="https://www.freecodecamp.org/news/css-tutorial-drop-shadow/">CSS Box Shadow</a>
                        <a href="https://www.freecodecamp.org/news/python-list-append-how-to-add-an-element-to-an-array-explained-with-examples/">Python
                            List Append</a>
                        <a href="https://www.freecodecamp.org/news/javascript-array-sort-tutorial-how-to-use-js-sort-methods-with-code-examples/">JavaScript
                            Array Sort</a>
                        <a href="https://www.freecodecamp.org/news/symlink-tutorial-in-linux-how-to-create-and-remove-a-symbolic-link/">Symlink
                            in Linux</a>
                        <a href="https://www.freecodecamp.org/news/grep-command-tutorial-how-to-search-for-a-file-in-linux-and-unix/">Linux
                            Grep Command</a>
                        <a href="https://www.freecodecamp.org/news/what-is-dns/">What is DNS?</a>
                        <a href="https://www.freecodecamp.org/news/primary-key-sql-tutorial-how-to-define-a-primary-key-in-a-database/">Primary
                            Key SQL</a>
                        <a href="https://www.freecodecamp.org/news/sql-update-statement-example-queries-for-updating-table-values/">SQL
                            Update Statement</a>
                        <a href="https://www.freecodecamp.org/news/how-to-screenshot-on-windows/">Screenshot on PC</a>
                    </div>
                    <div class="footer-col footer-col-2">
                        <a href="https://www.freecodecamp.org/news/javascript-es6-promises-for-beginners-resolve-reject-and-chaining-explained/">JavaScript
                            Promise</a>
                        <a href="https://www.freecodecamp.org/news/what-is-github-what-is-git-and-how-to-use-these-developer-tools/">What
                            is GitHub?</a>
                        <a href="https://www.freecodecamp.org/news/the-python-sort-list-array-method-ascending-and-descending-explained-with-examples/">Python
                            Sort List</a>
                        <a href="https://www.freecodecamp.org/news/json-comment-example-how-to-comment-in-json-files/">Comments
                            in JSON</a>
                        <a href="https://www.freecodecamp.org/news/what-is-kanban-the-agile-methodology-defined-and-how-to-use-it-for-your-software-development-team-2/">What
                            is Kanban?</a>
                        <a href="https://www.freecodecamp.org/news/python-write-to-file-open-read-append-and-other-file-handling-functions-explained/">Python
                            Write to File</a>
                        <a href="https://www.freecodecamp.org/news/css-media-queries-breakpoints-media-types-standard-resolutions-and-more/">CSS
                            Media Queries</a>
                        <a href="https://www.freecodecamp.org/news/html-entities-symbols-special-character-codes-list/">HTML
                            Entities</a>
                        <a href="https://www.freecodecamp.org/news/excel-vba-tutorial/">Excel VBA</a>
                        <a href="https://www.freecodecamp.org/news/vlookup-in-excel/">LOOKUP in Excel</a>
                    </div>
                    <div class="footer-col footer-col-3">
                        <div class="footer-left">
                            <a href="https://www.freecodecamp.org/news/what-is-a-proxy-server-in-english-please/">What
                                is a Proxy Server?</a>
                            <a href="https://www.freecodecamp.org/news/the-cat-command-in-linux-concatenation-explained-with-bash-examples/">Cat
                                Command in Linux</a>
                            <a href="https://www.freecodecamp.org/news/how-to-add-an-image-url-to-your-div/">CSS
                                Background Image</a>
                            <a href="https://www.freecodecamp.org/news/html-background-color-tutorial-how-to-change-a-div-background-color-explained-with-code-examples/">HTML
                                Background Color</a>
                            <a href="https://www.freecodecamp.org/news/comments-in-css/">CSS Comment Example</a>
                        </div>

                        <div class="footer-right">
                            <a href="https://www.freecodecamp.org/news/arrow-function-javascript-tutorial-how-to-declare-a-js-function-with-the-new-es6-syntax/">Arrow
                                Function JavaScript</a>
                            <a href="https://www.freecodecamp.org/news/how-to-remove-duplicates-in-excel-delete-duplicate-rows-with-a-few-clicks/">Remove
                                Duplicates in Excel</a>
                            <a href="https://www.freecodecamp.org/news/what-is-dllhost-exe-and-com-surrogate-in-windows-task-manager-solved/">dllhost.exe
                                COM Surrogate</a>
                            <a href="https://www.freecodecamp.org/news/boolean-algebra/">Boolean Algebra Truth Table</a>
                            <a href="https://www.freecodecamp.org/news/can-you-facetime-on-android-no-but-here-are-some-alternative-video-conferencing-apps/">Video
                                Chat for Android</a>

                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="footer-buttom">
            <div class="col-header">Our Nonprofit</div>
            <div class="footer-divder"></div>
            <div class="our-nonprofit">
                <a href="https://www.freecodecamp.org/news/about/">About</a>
                <a href="https://www.linkedin.com/school/free-code-camp/people/" rel="noopener noreferrer" target="_blank">Alumni Network</a>
                <a href="https://github.com/freeCodeCamp/">Open Source</a>
                <a href="https://www.freecodecamp.org/shop/" rel="noopener noreferrer" target="_blank">Shop</a>
                <a href="https://www.freecodecamp.org/news/support/">Support</a>
                <a href="https://www.freecodecamp.org/news/sponsors/">Sponsors</a>
                <a href="https://www.freecodecamp.org/news/academic-honesty-policy/">Academic Honesty</a>
                <a href="https://www.freecodecamp.org/news/code-of-conduct/">Code of Conduct</a>
                <a href="https://www.freecodecamp.org/news/privacy-policy/">Privacy Policy</a>
                <a href="https://www.freecodecamp.org/news/terms-of-service/">Terms of Service</a>
                <a href="https://www.freecodecamp.org/news/copyright-policy/">Copyright Policy</a>
            </div>
        </div>
    </div>
</footer>
    </div>


    <div style="width: 0px; height: 0px; position: fixed; left: 0px; top: 0px; overflow: hidden;"><iframe frameborder="0" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/application-sha256-23087b2eb05f9225d0f1e4a0c0cc758a379febf18209f0102c2a90f76f8f7f63.html" name="runkit-application" style="padding: 0px; margin: 0px; border: 0px; height: 100vh; width: 0px; background: transparent;"></iframe></div><script>
        var images = document.querySelectorAll('.kg-gallery-image img');
        images.forEach(function (image) {
            var container = image.closest('.kg-gallery-image');
            var width = image.attributes.width.value;
            var height = image.attributes.height.value;
            var ratio = width / height;
            container.style.flex = ratio + ' 1 0%';
        })
    </script>


    <script src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/jquery-3.2.1.min.js.download" integrity="sha256-hwg4gsxgFZhOsEEamdOYGBf13FyQuiTwlAQgxVSNgt4=" crossorigin="anonymous">
        </script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/jquery.fitvids.js.download"></script>

    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-unescaped-markup.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-markup-templating.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-bash.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-c.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-clojure.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-cpp.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-csharp.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-css.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-docker.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-elixir.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-erlang.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-git.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-go.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-graphql.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-haskell.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-java.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-javascript.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-json.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-jsx.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-kotlin.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-lua.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-markup.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-php.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-python.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-r.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-ruby.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-rust.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-scala.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-sql.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-swift.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-typescript.min.js.download"></script>
    <script type="text/javascript" src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/prism-yaml.min.js.download"></script>

    <script>
    $(document).ready(function () {
        // Start fitVids
        var $postContent = $(".post-full-content");
        $postContent.fitVids();
        // End fitVids
    });
</script>


    <script src="./How to Build and Train K-Nearest Neighbors and K-Means Clustering ML Models in Python_files/_(anM_aWQ9VUEtNTU0NDY1MzEtMjA)_" async=""></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-55446531-20');
</script>



</body></html>
