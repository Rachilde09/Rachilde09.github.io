                                                                                                                                                                                                                  # [Start Bootstrap - Clean Blog Jekyll](https://startbootstrap.com/themes/clean-blog-jekyll/) - Official Jekyll Version

[Clean Blog Jekyll](https://startbootstrap.com/themes/clean-blog-jekyll/) is a stylish, responsive blog theme for [Bootstrap](https://getbootstrap.com/) created by [Start Bootstrap](https://startbootstrap.com/). This theme features a blog homepage, about page, contact page, and an example post page along with a working contact form powered by [Formspree](https://formspree.io/).

This repository holds the official Jekyll version of the Clean Blog theme on Start Bootstrap!

## Preview

[![Clean Blog (Jekyll) Preview](https://startbootstrap.com/assets/img/screenshots/themes/clean-blog-jekyll.png)](http://StartBootstrap.github.io/startbootstrap-clean-blog-jekyll/)

**[View Live Preview](http://StartBootstrap.github.io/startbootstrap-clean-blog-jekyll/)**

## Installation & Setup

### Using RubyGems

When installing the theme using RubyGems, demo images, posts, and pages are not included. Follow the instructions below for complete setup.

1. (Optional) Create a new Jekyll site: `jekyll new my-site`
2. Replace the current theme in your `Gemfile` with `gem "jekyll-theme-clean-blog"`.
3. Install the theme (run the command inside your site directory): `bundle install`
4. Replace the current theme in your `_config.yml` file with `theme: jekyll-theme-clean-blog`.
5. Build your site: `bundle exec jekyll serve`

Assuming there are no errors and the site is building properly, follow these steps next:

1. Create the following pages if they do not exist already (or change the extension of existing markdown files from `.md` to `.html`):

   * `index.html` - set to `layout: home`
   * `about.html` - set to `layout: page`
   * `contact.html` - set to `layout: page`
   * `posts/index.html` - set to `layout: page` (you will also need to create a `posts` directory)

2. Configure the `index.html` front matter. Example:

    ```markdown
    ---
    layout: home
    background: '/PATH_TO_IMAGE'
    ---
    ```

3. Configure the `about.html`, `contact.html`, and `posts/index.html` front matter. Example:

    ```markdown
    ---
    layout: page
    title: Page Title
    description: This is the page description.
    background: '/PATH_TO_IMAGE'
    ---
    ```

4. For each post in the `_posts` directory, update the front matter. Example:

    ```markdown
    ---
    layout: post
    title: "Post Title"
    subtitle: "This is the post subtitle."
    date: YYYY-MM-DD HH:MM:SS
    background: '/PATH_TO_IMAGE'
    ---
    ```

    For reference, look at the [demo repository](https://github.com/StartBootstrap/startbootstrap-clean-blog-jekyll) to see how the files are set up.

5. Add the form to the `contact.html` page. Add the following code to your `contact.html` page:

    ```html
    <form name="sentMessage" id="contactForm" novalidate>
      <div class="control-group">
        <div class="form-group floating-label-form-group controls">
          <label>Name</label>
          <input type="text" class="form-control" placeholder="Name" id="name" required data-validation-required-message="Please enter your name.">
          <p class="help-block text-danger"></p>
        </div>
      </div>
      <div class="control-group">
        <div class="form-group floating-label-form-group controls">
          <label>Email Address</label>
          <input type="email" class="form-control" placeholder="Email Address" id="email" required data-validation-required-message="Please enter your email address.">
          <p class="help-block text-danger"></p>
        </div>
      </div>
      <div class="control-group">
        <div class="form-group col-xs-12 floating-label-form-group controls">
          <label>Phone Number</label>
          <input type="tel" class="form-control" placeholder="Phone Number" id="phone" required data-validation-required-message="Please enter your phone number.">
          <p class="help-block text-danger"></p>
        </div>
      </div>
      <div class="control-group">
        <div class="form-group floating-label-form-group controls">
          <label>Message</label>
          <textarea rows="5" class="form-control" placeholder="Message" id="message" required data-validation-required-message="Please enter a message."></textarea>
          <p class="help-block text-danger"></p>
        </div>
      </div>
      <br>
      <div id="success"></div>
      <div class="form-group">
        <button type="submit" class="btn btn-primary" id="sendMessageButton">Send</button>
      </div>
    </form>
    ```

    Make sure you have the `email` setting in your `_config.yml` file set to a working email address! Once this is set, fill out the form and then check your email, verify the email address using the link sent to you by Formspree, and then the form will be working!

6. Build your site: `bundle exec jekyll serve`

### Using Core Files

When using the core files, the demo images, posts, and pages are all included with the download. After following the instructions below, you can then go and change the content of the pages and posts.

1. [Download](https://github.com/StartBootstrap/startbootstrap-clean-blog-jekyll/archive/master.zip) or Clone the repository.
2. Update the following configuration settings in your `_config.yml` file:

    * `baseurl`
    * `url`
    * `title`
    * `email` (after setting this setting to a working email address, fill out the form on the contact page and send it - then check your email and verify the address and the form will send you messages when used)
    * `description`
    * `author`
    * `twitter_username` (Optional)
    * `facebook_username` (Optional)
    * `github_username` (Optional)
    * `linkedin_username` (Optional)
    * `instagram_username` (Optional)

3. Build your site: `bundle exec jekyll serve`

## Bugs and Issues

Have a bug or an issue with this template? [Open a new issue](https://github.com/StartBootstrap/startbootstrap-clean-blog-jekyll/issues) here on GitHub!

## About

Start Bootstrap is an open source library of free Bootstrap templates and themes. All of the free templates and themes on Start Bootstrap are released under the MIT license, which means you can use them for any purpose, even for commercial projects.

* <https://startbootstrap.com>
* <https://twitter.com/SBootstrap>

Start Bootstrap was created by and is maintained by **[David Miller](http://davidmiller.io/)**.

* <http://davidmiller.io>
* <https://twitter.com/davidmillerhere>
* <https://github.com/davidtmiller>

Start Bootstrap is based on the [Bootstrap](https://getbootstrap.com/) framework created by [Mark Otto](https://twitter.com/mdo) and [Jacob Thorton](https://twitter.com/fat).

## Copyright and License

Copyright 2013-2021 Start Bootstrap LLC. Code released under the [MIT](https://github.com/StartBootstrap/startbootstrap-clean-blog-jekyll/blob/master/LICENSE) license.
                                                                                                                                                                                                                                                    ./contact.html                                                                                      0000644 0000000 0000000 00000024202 15052763301 012234  0                                                                                                    ustar   root                            root                                                                                                                                                                                                                   <!DOCTYPE html>

<html>

<head>

  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">


  <title>
    ANGOR Nora
  </title>

  <meta name="description" content="A Blog Theme by Start Bootstrap">

  <link href='https://fonts.googleapis.com/css?family=Lora:400,700,400italic,700italic' rel='stylesheet' type='text/css'>
  <link href='https://fonts.googleapis.com/css?family=Open+Sans:300italic,400italic,600italic,700italic,800italic,400,300,600,700,800' rel='stylesheet' type='text/css'>

  <script src="https://use.fontawesome.com/releases/v5.15.3/js/all.js" crossorigin="anonymous"></script>

  <link rel="stylesheet" href="/assets/main.css">
  <link rel="canonical" href="https://rachilde09.github.io/contact.html">
  <link rel="alternate" type="application/rss+xml" title="ANGOR Nora" href="/feed.xml">

</head>


<body>

  <!-- Navigation -->
<nav class="navbar navbar-expand-lg navbar-light fixed-top" id="mainNav">
  <div class="container">
    <a class="navbar-brand" href="/">ANGOR Nora</a>
    <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse"
      data-target="#navbarResponsive" aria-controls="navbarResponsive" aria-expanded="false"
      aria-label="Toggle navigation">
      Menu
      <i class="fa fa-bars"></i>
    </button>
    <div class="collapse navbar-collapse" id="navbarResponsive">
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link" href="/">Accueil</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/about">Ã€ propos</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/projets">Projets</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/education">Ã‰ducation</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/experience">ExpÃ©rience</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/cv">CV</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="/contact">Contact</a>
        </li>
      </ul>
    </div>
  </div>
</nav>


  <style>
/* Mise en forme de la page contact */
body {
  margin: 0;
  padding: 0;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

/* Centrage vertical du bloc contact */
.contact-wrapper {
  display: flex;
  gap: 0;
  max-width: 1100px;
  margin: auto; /* centre horizontalement */
  padding: 60px 0; /* espace haut/bas */
  position: relative;
  align-items: flex-start;
}

/* Ligne verticale dÃ©gradÃ©e au centre */
.contact-wrapper::before {
  content: "";
  position: absolute;
  top: 0;
  bottom: 0;
  left: 50%;
  width: 6px;
  background: repeating-linear-gradient(
    to bottom,
    #4f46e5,
    #4f46e5 10px,
    #9333ea 10px,
    #9333ea 20px
  );
  border-radius: 3px;
  transform: translateX(-50%);
  z-index: 2;
}

.contact-wrapper .contact-card.big {
  flex: 1;
  background: #2c2c2c;
  border-radius: 0;
  padding: 30px;
  color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
}

.contact-wrapper .contact-card.big:first-child {
  border-radius: 12px 0 0 12px;
}

.contact-wrapper .contact-card.big:last-child {
  border-radius: 0 12px 12px 0;
  /* dÃ©passe vers le haut et le bas */
  margin-top: -30px;
  margin-bottom: -30px;
}

.contact-card .intro {
  margin-bottom: 30px;
  font-size: 1.1rem;
}

.contact-details {
  display: flex;
  flex-direction: column;
  gap: 25px;
}

.contact-item {
  display: flex;
  align-items: center;
  gap: 15px;
}

.contact-item .icon {
  font-size: 1.5rem;
  color: white;
  flex-shrink: 0;
}

.contact-item .info {
  display: flex;
  flex-direction: column;
}

.contact-item .info h3 {
  margin: 0 0 5px;
  font-size: 1.1rem;
  font-weight: bold;
  background: linear-gradient(135deg, #4f46e5, #9333ea);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

/* Lien email en blanc par dÃ©faut, dÃ©gradÃ© au survol */
.contact-item .info a {
  color: white;
  text-decoration: none;
  transition: all 0.3s ease;
}

.contact-item .info a:hover {
  background: linear-gradient(135deg, #4f46e5, #9333ea);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

/* IcÃ´nes sociaux */
.social-icons a {
  font-size: 1.3rem;
  margin-right: 12px;
  color: white;
  transition: color 0.3s ease;
}

.social-icons a:hover {
  color: #9333ea;
}

/* Carte image */
.image-card {
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.image-card img {
  max-width: 100%;
  max-height: 100%;
  border-radius: 12px;
  object-fit: cover;
}

/* Responsive */
@media (max-width: 900px) {
  .contact-wrapper {
    flex-direction: column;
    padding: 30px 20px;
  }

  .contact-wrapper::before {
    display: none;
  }

  .contact-wrapper .contact-card.big {
    border-radius: 12px;
    margin: 0;
  }
}
</style>

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<div class="contact-wrapper">

  <!-- Carte gauche -->
  <div class="contact-card big">
    <h2>Contactez-moi</h2>
    <p class="intro">Nâ€™hÃ©sitez pas Ã  me contacter pour toute opportunitÃ© ou collaboration.</p>

    <div class="contact-details">

      <!-- RÃ©seaux sociaux -->
      <div class="contact-item">
        <div class="icon"><i class="fas fa-share-alt"></i></div>
        <div class="info">
          <h3>RÃ©seaux sociaux</h3>
          <div class="social-icons">
            <a href="https://www.linkedin.com/in/nora-angor-rachilde-13a957261/" target="_blank"><i class="fab fa-linkedin"></i></a>
            <a href="https://github.com/Rachilde09" target="_blank"><i class="fab fa-github"></i></a>
          </div>
        </div>
      </div>

      <!-- Email -->
      <div class="contact-item">
        <div class="icon"><i class="fas fa-envelope"></i></div>
        <div class="info">
          <h3>Email</h3>
          <a href="mailto:rachilde09@gmail.com">rachilde09@gmail.com</a>
        </div>
      </div>

    </div>
  </div>

  <!-- Carte droite (image) -->
  <div class="contact-card big image-card">
    <img src="/img/bg-contact.jpg" alt="Mon image de contact">
  </div>

</div>








 <!-- Retire le footer de la page d'accueil ET de la page contact -->
  


  <script src="https://code.jquery.com/jquery-3.5.1.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@4.6.0/dist/js/bootstrap.bundle.min.js"></script>
<script src="/assets/vendor/startbootstrap-clean-blog/js/scripts.js"></script>

<script src="/assets/scripts.js"></script>


  <!-- Form Validation -->
  <script src="/assets/vendor/startbootstrap-clean-blog/js/jqBootstrapValidation.js"></script>
  <!-- Send Form -->
  <script>
    $(function () {

      $("#contactForm input,#contactForm textarea").jqBootstrapValidation({
        preventSubmit: true,
        submitError: function ($form, event, errors) {
          // additional error messages or events
        },
        submitSuccess: function ($form, event) {
          event.preventDefault(); // prevent default submit behaviour
          // get values from FORM
          var name = $("input#name").val();
          var email = $("input#email").val();
          var phone = $("input#phone").val();
          var message = $("textarea#message").val();
          var firstName = name; // For Success/Failure Message
          // Check for white space in name for Success/Fail message
          if (firstName.indexOf(' ') >= 0) {
            firstName = name.split(' ').slice(0, -1).join(' ');
          }
          $this = $("#sendMessageButton");
          $this.prop("disabled", true); // Disable submit button until AJAX call is complete to prevent duplicate messages
          $.ajax({
            url: "//formspree.io/your-email@example.com",
            type: "POST",
            data: {
              name: name,
              phone: phone,
              email: email,
              message: message
            },
            cache: false,
            success: function () {
              // Success message
              $('#success').html("<div class='alert alert-success'>");
              $('#success > .alert-success').html("<button type='button' class='close' data-dismiss='alert' aria-hidden='true'>&times;").append("</button>");
              $('#success > .alert-success').append("<strong>Your message has been sent. </strong>");
              $('#success > .alert-success').append('</div>');
              //clear all fields
              $('#contactForm').trigger("reset");
            },
            error: function () {
              // Fail message
              $('#success').html("<div class='alert alert-danger'>");
              $('#success > .alert-danger').html("<button type='button' class='close' data-dismiss='alert' aria-hidden='true'>&times;").append("</button>");
              $('#success > .alert-danger').append($("<strong>").text("Sorry " + firstName + ", it seems that my mail server is not responding. Please try again later!"));
              $('#success > .alert-danger').append('</div>');
              //clear all fields
              $('#contactForm').trigger("reset");
            },
            complete: function () {
              setTimeout(function () {
                $this.prop("disabled", false); // Re-enable submit button when AJAX call is complete
              }, 1000);
            }
          });
        },
        filter: function () {
          return $(this).is(":visible");
        }
      });

      $("a[data-toggle=\"tab\"]").click(function (e) {
        e.preventDefault();
        $(this).tab("show");
      });
    });

    /*When clicking on Full hide fail/success boxes */
    $('#name').focus(function () {
      $('#success').html('');
    });
  </script>



  <!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-XXXXXXXXX-X"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-XXXXXXXXX-X');
</script>



</body>

</html>
                                                                                                                                                                                                                                                                                                                                                                                              ./projets/                                                                                          0000755 0000000 0000000 00000000000 15052763301 011401  5                                                                                                    ustar   root                            root                                                                                                                                                                                                                   ./projets/index.html                                                                                0000644 0000000 0000000 00000002431 15052763274 013407  0                                                                                                    ustar   root                            root                                                                                                                                                                                                                   layout: page
title: projets
background: '/img/bg-post.jpg'
---

{% for post in paginator.posts %}

<article class="post-preview">
  <a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
    <h2 class="post-title">{{ post.title }}</h2>
    {% if post.subtitle %}
    <h3 class="post-subtitle">{{ post.subtitle }}</h3>
    {% else %}
    <h3 class="post-subtitle">{{ post.excerpt | strip_html | truncatewords: 15 }}</h3>
    {% endif %}
  </a>
  <p class="post-meta">Posted by
    {% if post.author %}
    {{ post.author }}
    {% else %}
    {{ site.author }}
    {% endif %}
    on {{ post.date | date: '%B %d, %Y' }} &middot; {% include read_time.html content=post.content %}
  </p>
</article>

<hr>

{% endfor %}

<!-- Pager -->
{% if paginator.total_pages > 1 %}

<div class="clearfix">

  {% if paginator.previous_page %}
  <a class="btn btn-primary float-left" href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr;
    Newer<span class="d-none d-md-inline"> Posts</span></a>
  {% endif %}

  {% if paginator.next_page %}
  <a class="btn btn-primary float-right" href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older<span class="d-none d-md-inline"> Posts</span> &rarr;</a>
  {% endif %}

</div>

{% endif %}
                                                                                                                                                                                                                                       ./bin/                                                                                              0000755 0000000 0000000 00000000000 15052763301 010463  5                                                                                                    ustar   root                            root                                                                                                                                                                                                                   ./bin/cibuild                                                                                       0000755 0000000 0000000 00000000031 15052763274 012027  0                                                                                                    ustar   root                            root                                                                                                                                                                                                                   bundle exec jekyll build
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       ./jekyll-theme-clean-blog.gemspec                                                                   0000644 0000000 0000000 00000001356 15052763274 015671  0                                                                                                    ustar   root                            root                                                                                                                                                                                                                   # frozen_string_literal: true

Gem::Specification.new do |spec|
  spec.name          = "jekyll-theme-clean-blog"
  spec.version       = "4.0.12"
  spec.authors       = ["Start Bootstrap"]
  spec.email         = ["feedback@startbootstrap.com"]

  spec.summary       = "A simple blog theme based on Bootstrap 4 by Start Bootstrap."
  spec.homepage      = "https://github.com/StartBootstrap/startbootstrap-clean-blog-jekyll"
  spec.license       = "MIT"

  spec.files         = `git ls-files -z`.split("\x0").select { |f| f.match(%r{^(assets|_layouts|_includes|_sass|LICENSE|README)}i) }

  spec.add_runtime_dependency "jekyll", ">= 3.8.5"

  spec.add_development_dependency "bundler", "~> 2.0.1"
  spec.add_development_dependency "rake", "~> 12.0"
end
                                                                                                                                                                                                                                                                                  ./feed.xml                                                                                          0000644 0000000 0000000 00000065170 15052763301 011351  0                                                                                                    ustar   root                            root                                                                                                                                                                                                                   <?xml version="1.0" encoding="utf-8"?><feed xmlns="http://www.w3.org/2005/Atom" ><generator uri="https://jekyllrb.com/" version="3.10.0">Jekyll</generator><link href="https://rachilde09.github.io/feed.xml" rel="self" type="application/atom+xml" /><link href="https://rachilde09.github.io/" rel="alternate" type="text/html" /><updated>2025-08-25T04:29:50+00:00</updated><id>https://rachilde09.github.io/feed.xml</id><title type="html">ANGOR Nora</title><subtitle>A Blog Theme by Start Bootstrap</subtitle><author><name>Start Bootstrap</name></author><entry><title type="html">Man must explore, and this is exploration at its greatest</title><link href="https://rachilde09.github.io/2020/01/31/man-must-explore.html" rel="alternate" type="text/html" title="Man must explore, and this is exploration at its greatest" /><published>2020-01-31T14:45:13+00:00</published><updated>2020-01-31T14:45:13+00:00</updated><id>https://rachilde09.github.io/2020/01/31/man-must-explore</id><content type="html" xml:base="https://rachilde09.github.io/2020/01/31/man-must-explore.html"><![CDATA[<p>Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.</p>

<p>Science cuts two ways, of course; its products can be used for both good and evil. But there's no turning back from science. The early warnings about technological dangers also come from science.</p>

<p>What was most significant about the lunar voyage was not that man set foot on the Moon but that they set eye on the earth.</p>

<p>A Chinese tale tells of some men sent to harm a young girl who, upon seeing her beauty, become her protectors rather than her violators. That's how I felt seeing the Earth for the first time. I could not help but love and cherish her.</p>

<p>For those who have seen the Earth from space, and for the hundreds and perhaps thousands more who will, the experience most certainly changes your perspective. The things that we share in our world are far more valuable than those which divide us.</p>

<h2 class="section-heading">The Final Frontier</h2>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<blockquote class="blockquote">The dreams of yesterday are the hopes of today and the reality of tomorrow. Science has not yet mastered prophecy. We predict too much for the next year and yet far too little for the next ten.</blockquote>

<p>Spaceflights cannot be stopped. This is not the work of any one man or even a group of men. It is a historical process which mankind is carrying out in accordance with the natural laws of human development.</p>

<h2 class="section-heading">Reaching for the Stars</h2>

<p>As we got further and further away, it [the Earth] diminished in size. Finally it shrank to the size of a marble, the most beautiful you can imagine. That beautiful, warm, living object looked so fragile, so delicate, that if you touched it with a finger it would crumble and fall apart. Seeing this has to change a man.</p>

<img class="img-fluid" src="https://source.unsplash.com/Mn9Fa_wQH-M/800x450" alt="Demo Image">
<span class="caption text-muted">To go places and do things that have never been done before â€“ thatâ€™s what living is all about.</span>

<p>Space, the final frontier. These are the voyages of the Starship Enterprise. Its five-year mission: to explore strange new worlds, to seek out new life and new civilizations, to boldly go where no man has gone before.</p>

<p>As I stand out here in the wonders of the unknown at Hadley, I sort of realize thereâ€™s a fundamental truth to our nature, Man must explore, and this is exploration at its greatest.</p>

<p>Placeholder text by <a href="http://spaceipsum.com/">Space Ipsum</a>. Photographs by <a href="https://unsplash.com/">Unsplash</a>.</p>]]></content><author><name>Start Bootstrap</name></author><summary type="html"><![CDATA[Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.]]></summary></entry><entry><title type="html">I believe every human has a finite number of heartbeats. I donâ€™t intend to waste any of mine.</title><link href="https://rachilde09.github.io/2020/01/31/heartbeats.html" rel="alternate" type="text/html" title="I believe every human has a finite number of heartbeats. I donâ€™t intend to waste any of mine." /><published>2020-01-31T03:45:13+00:00</published><updated>2020-01-31T03:45:13+00:00</updated><id>https://rachilde09.github.io/2020/01/31/heartbeats</id><content type="html" xml:base="https://rachilde09.github.io/2020/01/31/heartbeats.html"><![CDATA[<p>Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.</p>

<p>Science cuts two ways, of course; its products can be used for both good and evil. But there's no turning back from science. The early warnings about technological dangers also come from science.</p>

<p>What was most significant about the lunar voyage was not that man set foot on the Moon but that they set eye on the earth.</p>

<p>A Chinese tale tells of some men sent to harm a young girl who, upon seeing her beauty, become her protectors rather than her violators. That's how I felt seeing the Earth for the first time. I could not help but love and cherish her.</p>

<p>For those who have seen the Earth from space, and for the hundreds and perhaps thousands more who will, the experience most certainly changes your perspective. The things that we share in our world are far more valuable than those which divide us.</p>

<h2 class="section-heading">The Final Frontier</h2>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<blockquote class="blockquote">The dreams of yesterday are the hopes of today and the reality of tomorrow. Science has not yet mastered prophecy. We predict too much for the next year and yet far too little for the next ten.</blockquote>

<p>Spaceflights cannot be stopped. This is not the work of any one man or even a group of men. It is a historical process which mankind is carrying out in accordance with the natural laws of human development.</p>

<h2 class="section-heading">Reaching for the Stars</h2>

<p>As we got further and further away, it [the Earth] diminished in size. Finally it shrank to the size of a marble, the most beautiful you can imagine. That beautiful, warm, living object looked so fragile, so delicate, that if you touched it with a finger it would crumble and fall apart. Seeing this has to change a man.</p>

<img class="img-fluid" src="https://source.unsplash.com/Mn9Fa_wQH-M/800x450" alt="Demo Image">
<span class="caption text-muted">To go places and do things that have never been done before â€“ thatâ€™s what living is all about.</span>

<p>Space, the final frontier. These are the voyages of the Starship Enterprise. Its five-year mission: to explore strange new worlds, to seek out new life and new civilizations, to boldly go where no man has gone before.</p>

<p>As I stand out here in the wonders of the unknown at Hadley, I sort of realize thereâ€™s a fundamental truth to our nature, Man must explore, and this is exploration at its greatest.</p>

<p>Placeholder text by <a href="http://spaceipsum.com/">Space Ipsum</a>. Photographs by <a href="https://unsplash.com/">Unsplash</a>.</p>]]></content><author><name>Start Bootstrap</name></author><summary type="html"><![CDATA[Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.]]></summary></entry><entry><title type="html">Science has not yet mastered prophecy</title><link href="https://rachilde09.github.io/2020/01/30/prophecy.html" rel="alternate" type="text/html" title="Science has not yet mastered prophecy" /><published>2020-01-30T03:45:13+00:00</published><updated>2020-01-30T03:45:13+00:00</updated><id>https://rachilde09.github.io/2020/01/30/prophecy</id><content type="html" xml:base="https://rachilde09.github.io/2020/01/30/prophecy.html"><![CDATA[<p>Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.</p>

<p>Science cuts two ways, of course; its products can be used for both good and evil. But there's no turning back from science. The early warnings about technological dangers also come from science.</p>

<p>What was most significant about the lunar voyage was not that man set foot on the Moon but that they set eye on the earth.</p>

<p>A Chinese tale tells of some men sent to harm a young girl who, upon seeing her beauty, become her protectors rather than her violators. That's how I felt seeing the Earth for the first time. I could not help but love and cherish her.</p>

<p>For those who have seen the Earth from space, and for the hundreds and perhaps thousands more who will, the experience most certainly changes your perspective. The things that we share in our world are far more valuable than those which divide us.</p>

<h2 class="section-heading">The Final Frontier</h2>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<blockquote class="blockquote">The dreams of yesterday are the hopes of today and the reality of tomorrow. Science has not yet mastered prophecy. We predict too much for the next year and yet far too little for the next ten.</blockquote>

<p>Spaceflights cannot be stopped. This is not the work of any one man or even a group of men. It is a historical process which mankind is carrying out in accordance with the natural laws of human development.</p>

<h2 class="section-heading">Reaching for the Stars</h2>

<p>As we got further and further away, it [the Earth] diminished in size. Finally it shrank to the size of a marble, the most beautiful you can imagine. That beautiful, warm, living object looked so fragile, so delicate, that if you touched it with a finger it would crumble and fall apart. Seeing this has to change a man.</p>

<img class="img-fluid" src="https://source.unsplash.com/Mn9Fa_wQH-M/800x450" alt="Demo Image">
<span class="caption text-muted">To go places and do things that have never been done before â€“ thatâ€™s what living is all about.</span>

<p>Space, the final frontier. These are the voyages of the Starship Enterprise. Its five-year mission: to explore strange new worlds, to seek out new life and new civilizations, to boldly go where no man has gone before.</p>

<p>As I stand out here in the wonders of the unknown at Hadley, I sort of realize thereâ€™s a fundamental truth to our nature, Man must explore, and this is exploration at its greatest.</p>

<p>Placeholder text by <a href="http://spaceipsum.com/">Space Ipsum</a>. Photographs by <a href="https://unsplash.com/">Unsplash</a>.</p>]]></content><author><name>Start Bootstrap</name></author><summary type="html"><![CDATA[Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.]]></summary></entry><entry><title type="html">Failure is not an option</title><link href="https://rachilde09.github.io/2020/01/29/exploration.html" rel="alternate" type="text/html" title="Failure is not an option" /><published>2020-01-29T03:45:13+00:00</published><updated>2020-01-29T03:45:13+00:00</updated><id>https://rachilde09.github.io/2020/01/29/exploration</id><content type="html" xml:base="https://rachilde09.github.io/2020/01/29/exploration.html"><![CDATA[<p>Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.</p>

<p>Science cuts two ways, of course; its products can be used for both good and evil. But there's no turning back from science. The early warnings about technological dangers also come from science.</p>

<p>What was most significant about the lunar voyage was not that man set foot on the Moon but that they set eye on the earth.</p>

<p>A Chinese tale tells of some men sent to harm a young girl who, upon seeing her beauty, become her protectors rather than her violators. That's how I felt seeing the Earth for the first time. I could not help but love and cherish her.</p>

<p>For those who have seen the Earth from space, and for the hundreds and perhaps thousands more who will, the experience most certainly changes your perspective. The things that we share in our world are far more valuable than those which divide us.</p>

<h2 class="section-heading">The Final Frontier</h2>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<blockquote class="blockquote">The dreams of yesterday are the hopes of today and the reality of tomorrow. Science has not yet mastered prophecy. We predict too much for the next year and yet far too little for the next ten.</blockquote>

<p>Spaceflights cannot be stopped. This is not the work of any one man or even a group of men. It is a historical process which mankind is carrying out in accordance with the natural laws of human development.</p>

<h2 class="section-heading">Reaching for the Stars</h2>

<p>As we got further and further away, it [the Earth] diminished in size. Finally it shrank to the size of a marble, the most beautiful you can imagine. That beautiful, warm, living object looked so fragile, so delicate, that if you touched it with a finger it would crumble and fall apart. Seeing this has to change a man.</p>

<img class="img-fluid" src="https://source.unsplash.com/Mn9Fa_wQH-M/800x450" alt="Demo Image">
<span class="caption text-muted">To go places and do things that have never been done before â€“ thatâ€™s what living is all about.</span>

<p>Space, the final frontier. These are the voyages of the Starship Enterprise. Its five-year mission: to explore strange new worlds, to seek out new life and new civilizations, to boldly go where no man has gone before.</p>

<p>As I stand out here in the wonders of the unknown at Hadley, I sort of realize thereâ€™s a fundamental truth to our nature, Man must explore, and this is exploration at its greatest.</p>

<p>Placeholder text by <a href="http://spaceipsum.com/">Space Ipsum</a>. Photographs by <a href="https://unsplash.com/">Unsplash</a>.</p>]]></content><author><name>Start Bootstrap</name></author><summary type="html"><![CDATA[Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.]]></summary></entry><entry><title type="html">The dreams of yesterday are the hopes of today and the reality of tomorrow.</title><link href="https://rachilde09.github.io/2020/01/28/dreams.html" rel="alternate" type="text/html" title="The dreams of yesterday are the hopes of today and the reality of tomorrow." /><published>2020-01-28T03:45:13+00:00</published><updated>2020-01-28T03:45:13+00:00</updated><id>https://rachilde09.github.io/2020/01/28/dreams</id><content type="html" xml:base="https://rachilde09.github.io/2020/01/28/dreams.html"><![CDATA[<p>Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.</p>

<p>Science cuts two ways, of course; its products can be used for both good and evil. But there's no turning back from science. The early warnings about technological dangers also come from science.</p>

<p>What was most significant about the lunar voyage was not that man set foot on the Moon but that they set eye on the earth.</p>

<p>A Chinese tale tells of some men sent to harm a young girl who, upon seeing her beauty, become her protectors rather than her violators. That's how I felt seeing the Earth for the first time. I could not help but love and cherish her.</p>

<p>For those who have seen the Earth from space, and for the hundreds and perhaps thousands more who will, the experience most certainly changes your perspective. The things that we share in our world are far more valuable than those which divide us.</p>

<h2 class="section-heading">The Final Frontier</h2>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<blockquote class="blockquote">The dreams of yesterday are the hopes of today and the reality of tomorrow. Science has not yet mastered prophecy. We predict too much for the next year and yet far too little for the next ten.</blockquote>

<p>Spaceflights cannot be stopped. This is not the work of any one man or even a group of men. It is a historical process which mankind is carrying out in accordance with the natural laws of human development.</p>

<h2 class="section-heading">Reaching for the Stars</h2>

<p>As we got further and further away, it [the Earth] diminished in size. Finally it shrank to the size of a marble, the most beautiful you can imagine. That beautiful, warm, living object looked so fragile, so delicate, that if you touched it with a finger it would crumble and fall apart. Seeing this has to change a man.</p>

<img class="img-fluid" src="https://source.unsplash.com/Mn9Fa_wQH-M/800x450" alt="Demo Image">
<span class="caption text-muted">To go places and do things that have never been done before â€“ thatâ€™s what living is all about.</span>

<p>Space, the final frontier. These are the voyages of the Starship Enterprise. Its five-year mission: to explore strange new worlds, to seek out new life and new civilizations, to boldly go where no man has gone before.</p>

<p>As I stand out here in the wonders of the unknown at Hadley, I sort of realize thereâ€™s a fundamental truth to our nature, Man must explore, and this is exploration at its greatest.</p>

<p>Placeholder text by <a href="http://spaceipsum.com/">Space Ipsum</a>. Photographs by <a href="https://unsplash.com/">Unsplash</a>.</p>]]></content><author><name>Start Bootstrap</name></author><summary type="html"><![CDATA[Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.]]></summary></entry><entry><title type="html">Dinosaurs are extinct today</title><link href="https://rachilde09.github.io/2020/01/27/dinosaurs.html" rel="alternate" type="text/html" title="Dinosaurs are extinct today" /><published>2020-01-27T03:45:13+00:00</published><updated>2020-01-27T03:45:13+00:00</updated><id>https://rachilde09.github.io/2020/01/27/dinosaurs</id><content type="html" xml:base="https://rachilde09.github.io/2020/01/27/dinosaurs.html"><![CDATA[<p>Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.</p>

<p>Science cuts two ways, of course; its products can be used for both good and evil. But there's no turning back from science. The early warnings about technological dangers also come from science.</p>

<p>What was most significant about the lunar voyage was not that man set foot on the Moon but that they set eye on the earth.</p>

<p>A Chinese tale tells of some men sent to harm a young girl who, upon seeing her beauty, become her protectors rather than her violators. That's how I felt seeing the Earth for the first time. I could not help but love and cherish her.</p>

<p>For those who have seen the Earth from space, and for the hundreds and perhaps thousands more who will, the experience most certainly changes your perspective. The things that we share in our world are far more valuable than those which divide us.</p>

<h2 class="section-heading">The Final Frontier</h2>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<p>There can be no thought of finishing for â€˜aiming for the stars.â€™ Both figuratively and literally, it is a task to occupy the generations. And no matter how much progress one makes, there is always the thrill of just beginning.</p>

<blockquote class="blockquote">The dreams of yesterday are the hopes of today and the reality of tomorrow. Science has not yet mastered prophecy. We predict too much for the next year and yet far too little for the next ten.</blockquote>

<p>Spaceflights cannot be stopped. This is not the work of any one man or even a group of men. It is a historical process which mankind is carrying out in accordance with the natural laws of human development.</p>

<h2 class="section-heading">Reaching for the Stars</h2>

<p>As we got further and further away, it [the Earth] diminished in size. Finally it shrank to the size of a marble, the most beautiful you can imagine. That beautiful, warm, living object looked so fragile, so delicate, that if you touched it with a finger it would crumble and fall apart. Seeing this has to change a man.</p>

<img class="img-fluid" src="https://source.unsplash.com/Mn9Fa_wQH-M/800x450" alt="Demo Image">
<span class="caption text-muted">To go places and do things that have never been done before â€“ thatâ€™s what living is all about.</span>

<p>Space, the final frontier. These are the voyages of the Starship Enterprise. Its five-year mission: to explore strange new worlds, to seek out new life and new civilizations, to boldly go where no man has gone before.</p>

<p>As I stand out here in the wonders of the unknown at Hadley, I sort of realize thereâ€™s a fundamental truth to our nature, Man must explore, and this is exploration at its greatest.</p>

<p>Placeholder text by <a href="http://spaceipsum.com/">Space Ipsum</a>. Photographs by <a href="https://unsplash.com/">Unsplash</a>.</p>]]></content><author><name>Start Bootstrap</name></author><summary type="html"><![CDATA[Never in all their history have men been able truly to conceive of the world as one: a single sphere, a globe, having the qualities of a globe, a round earth in which all the directions eventually meet, in which there is no center because every point, or none, is center â€” an equal earth which all men occupy as equals. The airman's earth, if free men make it, will be truly round: a globe in practice, not in theory.]]></summary></entry></feed>                                                                                                                                                                                                                                                                                                                                                                                                        ./img/                                                                                              0000755 0000000 0000000 00000000000 15052763301 010467  5                                                                                                    ustar   root                            root                                                                                                                                                                                                                   ./img/bg-contact.jpg                                                                                0000644 0000000 0000000 00001721710 15052763274 013234  0                                                                                                    ustar   root                            root                                                                                                                                                                                                                   ÿØÿá Exif  II*            ÿì Ducky     d  ÿáhttp://ns.adobe.com/xap/1.0/ <?xpacket begin="ï»¿" id="W5M0MpCehiHzreSzNTczkc9d"?> <x:xmpmeta xmlns:x="adobe:ns:meta/" x:xmptk="Adobe XMP Core 5.6-c140 79.160451, 2017/05/06-01:08:21        "> <rdf:RDF xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"> <rdf:Description rdf:about="" xmlns:xmpMM="http://ns.adobe.com/xap/1.0/mm/" xmlns:stRef="http://ns.adobe.com/xap/1.0/sType/ResourceRef#" xmlns:xmp="http://ns.adobe.com/xap/1.0/" xmpMM:DocumentID="xmp.did:7F15AA45B6A411E7AA3CA766BD1EAA4B" xmpMM:InstanceID="xmp.iid:7F15AA44B6A411E7AA3CA766BD1EAA4B" xmp:CreatorTool="Adobe Photoshop CC 2018 Macintosh"> <xmpMM:DerivedFrom stRef:instanceID="6A236A045F985AD817D32BAE43427E45" stRef:documentID="6A236A045F985AD817D32BAE43427E45"/> </rdf:Description> </rdf:RDF> </x:xmpmeta> <?xpacket end="r"?>ÿî Adobe dÀ   ÿÛ „ ÿÀ ól ÿÄ “             	
                   !1AQaq‘¡"	ð±ÁÑ2áñB#
Rb$r3‚’%¢C²Ò4Â&S5csóTe'                ÿÚ   ? ÷‹þ.Ì§ÈÓ†+~ Žòh:|™Á•s‰…W>s ÓfÚ<çû–r!Ut<rÇ¾Cµ4›9[5µ•¬2°Í,iB„âÜT¥¿- Ùâ½üh+Ð@—<8(ö@è
€ (>ÿ Â‚(iŽ`1üh C€Ä|M2ª¹ãÜ|2 ¸c°
}Ùw÷çA_1‡q*@ûÒx}¾Þ û{()—ˆŽõì ˆÌ¢Œ²ãAP¨BvxøähI#×Â¦}á>ÿ ÎÐ&+ØSÆPùÿ  ´^Ü±Ä{Žt
‚Jˆ8ƒíA…íûqø|0 (
‡îñ 8dWá÷P0½Ô
€ ©ÌäTñNŸÂb§±;ÿ A%DE*©ÍöÐ$„Nÿ Ò¸q^	J!#q÷qÄh)û=¿l('Î{¾ÞÚŠ)%3^(¸P6©%p<Jb{QÂüÊÁ0NdÅ|€OË‡³QÛA­8‰*Wì  ¡#+šâ~4P}½¼}ùÐ Œ‡d(
€ ;¾Ü?*€ (L¨
ŒÇ gòû¨$×aËrgšÐ6
H
Š½´$ ãŠÐ‰
1?ÊNä<pO à(Šû0ñJ¢g@Ê`|h#|( S@ù—Á÷¦Y~4o6
pÇ<Ïã…Ô®9c»Ý@×
dPrã@qÓø~4€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ ()ÀŸ ´]¸‘À÷ºÐ ª{%öû>ØÐ@P@P#†$á@ûèåÙ˜ñí 8§øö{¨"õN=ý™ýôi# žðï ©*…FK€öPRqROÛð _lè
ì_àE (
€ (
€ `•ƒ1øPT0€ ‹‡0J
*îÄÍ€jâP’ƒ 3à¦ƒBÿ KçyÜá99|„o—ÍÍÍÎ«Íæ/N\(5ÐPþ ãáÜ($\Q2eØ™PEJ'@¨¶t@P,
@@Æ8Ð@»/¾Ð¾Â´*[ˆ\òíR²‚ŒB	Ü™­i 'BžøöP]0áÃØ¼|h'í_·} {³ ¢å%P§…!¹>8ÐL Pràq*sCÁ;ÂŠPP¦|>Þ%xb;2ÁrZì?Î€N<((ÀpË†t
€ >ßlh%ÀaÚ¥3Çî @P@P@Á#—²€^áöøP?”˜â¼p;( sTÅqNÜø.T“€9p T
1O‘QÞÙŠ	—PÈiO†T	J…i@ˆá–T
Tâ)DÁ1 ‘ œ0öŸçAL’Pœsü;€hSÜ8PHAQ— È aÀ(+™DCŸ8Ð!úpËnÿ e¸’rÁ1Àa ;0à˜æ´®	Û…Zíã@P@PoÃíá@Pl“î (ß•@ÁW>ÆP3÷w{þ4Ìøš‚{†? (
¨T}¾ú
€’2æÄŒÀà($… ™®_nïÆÐàGˆJSÞ‚Ž4€ (
€îûqü¨
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ùÐñþ
€ Ex?ÊŽðÔïÄ{ RÐ,||€ 3Ìà$4
W*íŸá•UNð¿wç@`Þ'ï DŒ8öÜ1Ç‰oyNÄ8b§%÷-ÄŒ¨û¨ AûcÙ@ }» =¨´,Oð%8ªp=¨h2ªâ8O~+W»Á?<è$P
žìò …@P@P
'óáA.CÄ„ ˜`¾Ôü¨Vö}ô haöïSA*€ (Îÿ å@P<¹~9	Ä
@PìîüÉüh@'4 (·Û
O™üŽ4wç@P œ±ÀzcÆ‚>[±QÀcŽ<8Ð!‡p'ð ®ÆBð…ZŽÝ@¹G;x¨â(å†a|2ÂÐ?ÛÛ@¨
ŽKñAùPM¡ãÞ‡óÃ°PE?6]Ùøc@“.Â˜ð÷Ð.ïº•È¯¶€Ç‡?¹:@P@P0S€>4â1ñ@¨)‚§Ò€LíÇ} 18gÃÙ Fkšâ<qZOyÀýÔáh•°ÍG‚Ð
L^Ã•Áæî„_Ô¼8e@¿J€{qæ‹A&•‡wge]‰ åŠŸÃá@ÔO»=Ë@UR™þ	@‚rêØ~ä4åP3ììÇÚ	rŒÑq)øPKÃî Gñ´pÙ@è
€ (
€ >ß}@P·¿óð TgöÃý”àê´¯w€þ4¦Kã—ÂP
NE|;8|(APsÂâ9:	®(žÞÎ€%8ãüèÐ¨OàFk@˜öàx_½hÛ¶¡;~ÙP:€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ i?Ç…ƒg‡–]´L»‚'»ò d(Êò7³â:‘¿Ã‘´#pÀ`¾8÷­ÈÞÏ‰ \ƒ¿áùP//¿áüh!îøþT!îûvP‡»ãùP.G¶4ä<OãùP_~4öŠ÷P‡»ãùP.Gv|Gç@r;³â?:B1@¨Ãî öu (
€ (
€ r (
€ (
 ™w~?ž`'Û‚PÁÇòª÷®>ä ¤A®4gwæOwm
¿/Û‡ãAQ
ð/.Â¦$öþCò \¨BÉìÌq 	ùJ÷ŠP à‡!‚œ
ó ˆÑùgÝ@92ïUçÝ‡m8ãÅ>4ïû×ã@¨
€ (
€ a¤ü=‹ÝAT0Èþ4 (
€ (•U'?bŽ
€ (
ƒHÃJgùÐ/¶K÷Ð÷w}Øüh@P@PÃ´øPA6¹£6…ÌSAT88píà†!íUã—€þ4åniöðÊ€åiáø}Ô- éÞ8 §‚÷aüh ŠP!ø‚
 p^ê€ (
ÌQ
@×…^4.ÈñAÝ@›ú‚öžìO… J§þ‘÷þt.ÀqÇ²€Ã.ü×º€É}€§¿ð š` ¨Ç.ÊbžpQøÐH f‰ñC@€OÔ
pÏ:Z™àŠŸ}ÉŠ¡öæ0ï E¥cÜ‰÷÷ÐLž8w'à€ fŠxÿ .4 
$àGŠ…^å 9q*0Ë‰%r¾€ä­yr-Ä’pã¹Giø~T
Æ9¦ššˆpãÜ¹xe@&|Ø‚T{“Új…O~g)• ?QÀ¢¨î)ŠûèŸ¸'9­ ½ÇáùÐ:³Çqüh
€ (
€ (
€ ‘i0^Ì$ ohÀŽ–4'zööû3Æ‚<‡ùý¹|Hüm f>RpB3ííLèCÃÏ#@¹pUãØ% HÁ
öŒ¾êÊsJ8eŸßA$$…NÓ‚xð@œ1Ã#’cã@ƒIÈPT¨„pÃÛA ¸¯iO€ H;ó\Ïç@è
€ =«öî (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (
€ (

