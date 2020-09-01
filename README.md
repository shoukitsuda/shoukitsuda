# profile
hello!

<div class="wrapper">
  <ul class="share">
    <li class="twitter"><a href="https://twitter.com/intent/tweet?url=[URL]&text=[TITLE]&via=[USER]" target="_blank"><span class="entypo-twitter"></span></a></li>
    <li class="facebook"><a href="https://www.facebook.com/share.php?u=[URL]&t=[TITLE]" target="_blank"><span class="entypo-facebook"></span></a></li>
    <li class="linkedin"><a href="https://www.linkedin.com/shareArticle?mini=true&url=[URL]&title=[TITLE]&source=[SOURCE]" target="_blank"><span class="entypo-linkedin"></span></a></li>
    <li class="googleplus"><a href="https://plus.google.com/share?url=[URL]" target="_blank"><span class="entypo-gplus"></span></a></li>
  </ul>
</div>

$twitter: #00aced;
$facebook: #3b5998;
$linkedin: #0977b5;
$googleplus: #cc3732;

@import url(http://weloveiconfonts.com/api/?family=entypo);

/* entypo */
[class*="entypo-"]::before {
  font-family: 'entypo', sans-serif;
}

* {
  box-sizing: border-box;
}

.wrapper {
  width: 80%;
  height: 100%;
  margin: 0 auto;
}

.share {
  position: absolute;
  top: 50%;
  left: 50%;
  font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  font-size: 1em;
  margin-top: -17px;
  margin-left: -70px;
  font-weight: 700;
  text-align: center;
  span { font-weight: 400; }
  li {
    display: inline-block;
    a {
      display: block;
      width: 32px;
      color: #fff;
      text-decoration: none;
      border-bottom-width: 4px;
      border-bottom-style: solid;
      border-radius: 3px;
      padding: 6px 0;
      transition: .025s all ease-in-out;
      &:active {
        border-bottom: 0;
        box-shadow: inset 0 4px 4px rgba(0,0,0, .025);
        transform: translateY(4px);
      }
    }
    &.twitter a {
      background-color: $twitter;
      border-color: darken($twitter, 10%);
      &:hover,
      &:focus {
        background-color: lighten($twitter, 10%);
        border-color: $twitter;
      }
      &:active {
        background-color: darken($twitter, 10%);
      }
    }
    &.facebook a {
      background-color: $facebook;
      border-color: darken($facebook, 10%);
      &:hover,
      &:focus {
        background-color: lighten($facebook, 10%);
        border-color: $facebook;
      }
       &:active {
        background-color: darken($facebook, 10%);
      }
    }
    &.linkedin a {
      background-color: $linkedin;
      border-color: darken($linkedin, 10%);
      &:hover,
      &:focus {
        background-color: lighten($linkedin, 10%);
        border-color: $linkedin;
      }
       &:active {
        background-color: darken($linkedin, 10%);
      }
    }
    &.googleplus a {
      background-color: $googleplus;
      border-color: darken($googleplus, 10%);&:hover,
      &:hover,
      &:focus {
        background-color: lighten($googleplus, 10%);
        border-color: $googleplus;
      }
       &:active {
        background-color: darken($googleplus, 10%);
      }
    }
  }
}
