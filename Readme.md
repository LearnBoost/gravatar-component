
# gravatar

  Generate client-side gravatars. [Testing
  page](http://learnboost.github.io/gravatar-component/).

## Installation

    $ component install learnboost/gravatar-component

## API

### options

Most API calls take an option used to configure the url.

Options are the query string parameters described in the gravatar [documentation](https://en.gravatar.com/site/implement/images/)

  * **s** - size
  * **d** - default image `url` or {`404`,`mm`,`identicon`,`monsterid`,`wavatar`,`retro`,`blank`}
  * **r** - one of {`g`,`pg`,`r`,`x`}
  * **forcedefault** - force default image

### .url(email, options)

Return the gravatar image url for an email

### .img(email, options)

Creates an avatar `<img>` element

### .profile(email, callback(err, profile))

Looks up a profile

### .username(email, callback(err, username))

Shortcut that calls `.profile` to get a username from an email.

## Test

* Build example component doing `make`
* Open `test/index.html` file

## License

  MIT
