# Changelog

All notable changes to this project will be documented in this file, in reverse chronological order by release.

## 2.16.1 - TBD

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- Nothing.

## 2.16.0 - 2021-12-17


-----

### Release Notes for [2.16.0](https://github.com/laminas/laminas-feed/milestone/13)

Feature release (minor)

### 2.16.0

- Total issues resolved: **0**
- Total pull requests resolved: **1**
- Total contributors: **1**

#### Enhancement

 - [46: Mark more interface method returns with `#&#91;ReturnTypeWillChange&#93;` for PHP 8.1 compatibility](https://github.com/laminas/laminas-feed/pull/46) thanks to @Crell

## 2.15.0 - 2021-09-20


-----

### Release Notes for [2.15.0](https://github.com/laminas/laminas-feed/milestone/10)

Feature release (minor)

### 2.15.0

- Total issues resolved: **0**
- Total pull requests resolved: **2**
- Total contributors: **2**

#### Enhancement

 - [42: Provide PHP 8.1 support](https://github.com/laminas/laminas-feed/pull/42) thanks to @weierophinney

#### Duplicate,Enhancement

 - [39: Remove file headers](https://github.com/laminas/laminas-feed/pull/39) thanks to @ghostwriter

## 2.14.0 - 2021-03-16


-----

### Release Notes for [2.14.0](https://github.com/laminas/laminas-feed/milestone/7)

### Added

- Adds a new `PodcastIndex` extension to each of the Reader and Writer subcomponents, allowing users to both create and consume [xmlns:podcast feeds](https://github.com/Podcastindex-org/podcast-namespace/blob/main/docs/1.0.md). Please [read the documentation for more details](https://docs.laminas.dev/laminas-feed/extensions/podcast-index/).

### 2.14.0

- Total issues resolved: **0**
- Total pull requests resolved: **2**
- Total contributors: **2**

#### Enhancement

 - [35: Switch from Travis-CI to GitHub Actions](https://github.com/laminas/laminas-feed/pull/35) thanks to @weierophinney
 - [31: Create PodcastIndex extension](https://github.com/laminas/laminas-feed/pull/31) thanks to @codedmonkey

## 2.13.1 - 2021-01-04

### Fixed

- [#33](https://github.com/laminas/laminas-feed/pull/33) fixes an issue whereby parsing a feed entry date that is in an incorrect format was incorrectly causing a `null` value to be returned for the date, rather than correctly throwing an exception.

-----

### Release Notes for [2.13.1](https://github.com/laminas/laminas-feed/milestone/6)

2.13.x bugfix release (patch)

### 2.13.1

- Total issues resolved: **1**
- Total pull requests resolved: **1**
- Total contributors: **2**

#### Bug

- [33: Fixes 32 - Method getDateModified of RSS reader doesn't iterate over different formats](https://github.com/laminas/laminas-feed/pull/33) thanks to @froschdesign
- [32: Method getDateModified of RSS reader doesn't iterate over different formats](https://github.com/laminas/laminas-feed/issues/32) thanks to @Klaasie

## 2.13.0 - 2020-11-18

### Added

- [#28](https://github.com/laminas/laminas-feed/pull/28) Adds Psalm as QA tool
- [#29](https://github.com/laminas/laminas-feed/pull/29) Adds PHP 8.0 support

### Removed

- [#29](https://github.com/laminas/laminas-feed/pull/29) Dropped support for laminas-servicemanager less than v3.3


-----

### Release Notes for [2.13.0](https://github.com/laminas/laminas-feed/milestone/2)

next feature release (minor)

### 2.13.0

- Total issues resolved: **0**
- Total pull requests resolved: **2**
- Total contributors: **1**

#### Enhancement,hacktoberfest-accepted

 - [29: Update to support PHP 8.0](https://github.com/laminas/laminas-feed/pull/29) thanks to @ocean
 - [28: Add Psalm integration](https://github.com/laminas/laminas-feed/pull/28) thanks to @ocean

## 2.12.3 - 2020-08-18

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [#21](https://github.com/laminas/laminas-feed/pull/21) fixes the writer extension
  of iTunes to support valid values for the `itunes:explicit` element.

## 2.12.2 - 2020-03-29

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- Fixed `replace` version constraint in composer.json so repository can be used as replacement of `zendframework/zend-feed:^2.12.0`.

## 2.12.1 - 2020-03-23

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [#17](https://github.com/laminas/laminas-feed/pull/17) fixes regular expression to extract content from atom feeds.

## 2.12.0 - 2019-03-05

### Added

- [zendframework/zend-feed#96](https://github.com/zendframework/zend-feed/pull/96) adds the methods `Laminas\Feed\Reader\Extension\Podcast\Entry::getTitle() : string`
  and `Laminas\Feed\Writer\Extension\ITunes\Entry::setTitle(string $value)`; these
  provide the ability to read and manipulate `<itunes:title>` tags in feeds.

### Changed

- Nothing.

### Deprecated

- [zendframework/zend-feed#101](https://github.com/zendframework/zend-feed/pull/101) deprecates the method `Laminas\Feed\Writer\Writer::lcfirst()`; use the PHP
  built-in function instead.

- [zendframework/zend-feed#97](https://github.com/zendframework/zend-feed/pull/97) deprecates the classes `Laminas\Feed\Reader\AbstractEntry` (use
  `Laminas\Feed\Reader\Entry\AbstractEntry` instead), `Laminas\Feed\Reader\AbstractFeed` (use `Laminas\Feed\Reader\Feed\AbstractFeed` instead), and
  `Laminas\Feed\Reader\Collection` (use Laminas\Feed\Reader\Collection\Author`, `Laminas\Feed\Reader\Collection\Category`, or
  `Laminas\Feed\Reader\Collection\Collection` instead, based on context).

### Removed

- Nothing.

### Fixed

- Nothing.

## 2.11.1 - 2019-03-05

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-feed#99](https://github.com/zendframework/zend-feed/pull/99) provides a fix to `Laminas\Feed\Writer\Renderer\Entry\Rss` to ensure that
  relative URIs provided for the feed disable the `isPermalink` flag.

- [zendframework/zend-feed#100](https://github.com/zendframework/zend-feed/pull/100) fixes parameter and return value annotations for a number of classes to
  specify the correct types.

## 2.11.0 - 2019-01-29

### Added

- [zendframework/zend-feed#94](https://github.com/zendframework/zend-feed/pull/94) adds support for PHP 7.3.

- [zendframework/zend-feed#91](https://github.com/zendframework/zend-feed/pull/91) adds explicit requirements for both ext-dom and ext-libxml to the package.

### Changed

- [zendframework/zend-feed#93](https://github.com/zendframework/zend-feed/pull/93) `Writer\Feed`, `Writer\Entry` and `Writer\Deleted` all now accept
  `DateTimeImmutable` instances as an arguments to methods that previously only
  accepted `DateTime` or Unix Timestamps, such as `Writer\Feed::setDateModified()`.

### Deprecated

- Nothing.

### Removed

- [zendframework/zend-feed#94](https://github.com/zendframework/zend-feed/pull/94) removes support for laminas-stdlib v2 releases.

### Fixed

- Nothing.

## 2.10.3 - 2018-08-01

### Added

- Nothing.

### Changed

- This release modifies how `Laminas\Feed\Pubsubhubbub\AbstractCallback::_detectCallbackUrl()`
  marshals the request URI. In prior releases, we would attempt to inspect the
  `X-Rewrite-Url` and `X-Original-Url` headers, using their values, if present.
  These headers are issued by the ISAPI_Rewrite module for IIS (developed by
  HeliconTech). However, we have no way of guaranteeing that the module is what
  issued the headers, making it an unreliable source for discovering the URI. As
  such, we have removed this feature in this release.

  The method is not called internally. If you are calling the method from your
  own extension and need support for ISAPI_Rewrite, you will need to override
  the method as follows:

  ```php
  protected function _detectCallbackUrl()
  {
      $callbackUrl = null;
      if (isset($_SERVER['HTTP_X_REWRITE_URL'])) {
          $callbackUrl = $_SERVER['HTTP_X_REWRITE_URL'];
      }
      if (isset($_SERVER['HTTP_X_ORIGINAL_URL'])) {
          $callbackUrl = $_SERVER['HTTP_X_ORIGINAL_URL'];
      }

      return $callbackUrl ?: parent::__detectCallbackUrl();
  }
  ```

  If you use an approach such as the above, make sure you also instruct your web
  server to strip any incoming headers of the same name so that you can
  guarantee they are issued by the ISAPI_Rewrite module.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- Nothing.

## 2.10.2 - 2018-06-18

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-feed#81](https://github.com/zendframework/zend-feed/pull/81) updates the `Laminas\Feed\Reader\Reader` and `Laminas\Feed\Writer\Writer` classes to
  conditionally register their respective "GooglePlayPodcast" extensions only if
  their extension managers are aware of it. This is done due to the fact that
  existing `ExtensionManagerInterface` implementations may not register it by
  default as the extension did not exist in releases prior to 2.10.0. By having
  the registration conditional, we prevent an exception from being raised; users
  are not impacted by its absence, as the extension features were not exposed
  previously.
  
  Both `Reader` and `Writer` emit an `E_USER_NOTICE` when the extension is not
  found in the extension manager, indicating that the
  `ExtensionManagerInterface` implementation should be updated to add entries
  for the "GooglePlayPodcast" entry, feed, and/or renderer classes.

## 2.10.1 - 2018-06-05

### Added

- Nothing.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-feed#79](https://github.com/zendframework/zend-feed/pull/79) fixes an issue in the `setType()` method of the iTunes feed renderer whereby it was setting
  the DOM content with an uninitialized variable.

## 2.10.0 - 2018-05-24

### Added

- [zendframework/zend-feed#78](https://github.com/zendframework/zend-feed/pull/78) adds support for the Google Play Podcasts 1.0 DTD in both the Reader and
  Writer subcomponents. The following new classes provide the support:

  - `Laminas\Feed\Reader\Extension\GooglePlayPodcast\Entry`
  - `Laminas\Feed\Reader\Extension\GooglePlayPodcast\Feed`
  - `Laminas\Feed\Writer\Extension\GooglePlayPodcast\Entry`
  - `Laminas\Feed\Writer\Extension\GooglePlayPodcast\Feed`
  - `Laminas\Feed\Writer\Extension\GooglePlayPodcast\Renderer\Entry`
  - `Laminas\Feed\Writer\Extension\GooglePlayPodcast\Renderer\Feed`

  The extensions are registered by default with both `Laminas\Feed\Reader\Reader`
  and `Laminas\Feed\Writer\Writer`.

- [zendframework/zend-feed#77](https://github.com/zendframework/zend-feed/pull/77) adds support for `itunes:image` for each of:
  - `Laminas\Feed\Reader\Extension\Podcast\Entry`, via `getItunesImage()`; previously only the `Feed` supported it.
  - `Laminas\Feed\Writer\Extension\ITunes\Entry`, via `setItunesImage()`; previously only the `Feed` supported it.
  - `Laminas\Feed\Writer\Extension\ITunes\Renderer\Entry`; previously on the `Feed` supported it.

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Writer\Extension\ITunes\Entry::setItunesSeason()`, corresponding to the
  `itunes:season` tag, and allowing setting the season number of the episode the
  entry represents.

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Writer\Extension\ITunes\Entry::setItunesIsClosedCaptioned()`, corresponding to the
  `itunes:isClosedCaptioned` tag, and allowing setting the status of closed
  captioning support in the episode the entry represents.

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Writer\Extension\ITunes\Entry::setItunesEpisodeType()`, corresponding to the
  `itunes:episodeType` tag, and allowing setting the type of episode the entry represents
  (one of "full", "trailer", or "bonus", and defaulting to "full").

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Writer\Extension\ITunes\Entry::setEpisode()`, corresponding to the
  `itunes:episode` tag, and allowing setting the number of the episode the entry represents.

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Writer\Extension\ITunes\Feed::setItunesComplete()`, corresponding to the
  `itunes:complete` tag. It allows setting a boolean flag, indicating whether or not the
  podcast is complete (will not air new episodes).

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Writer\Extension\ITunes\Feed::setItunesType()`, corresponding to the
  `itunes:type` tag, and allowing setting the podcast type (one of "serial" or "episodic").

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Reader\Extension\Podcast\Entry::getEpisodeType()`, corresponding to the
  `itunes:episodeType` tag, and returning the type of episode the entry represents
  (one of "full", "trailer", or "bonus", and defaulting to "full").

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Reader\Extension\Podcast\Entry::getSeason()`, corresponding to the
  `itunes:season` tag, and returning the season number of the episode the entry represents.

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Reader\Extension\Podcast\Entry::isClsoedCaptioned()`, corresponding to the
  `itunes:isClosedCaptioned` tag, and returning the status of closed captioning
  in the episode the entry represents.

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Reader\Extension\Podcast\Entry::getEpisode()`, corresponding to the
  `itunes:episode` tag, and returning the number of the episode the entry represents.

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Reader\Extension\Podcast\Feed::isComplete()`, corresponding to the
  `itunes:complete` tag. It returns a boolean, indicating whether or not the podcast is
  complete (will not air new episodes).

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) adds `Laminas\Feed\Reader\Extension\Podcast\Feed::getPodcastType()`, corresponding to the
  `itunes:type` tag, and providing the podcast type (one of "serial" or "episodic", defaulting
  to the latter).

### Changed

- [zendframework/zend-feed#77](https://github.com/zendframework/zend-feed/pull/77) updates URI validation for `Laminas\Feed\Writer\Extension\ITunes\Feed::setItunesImage()` to
  first check that we have received a string value before proceeding.

### Deprecated

- [zendframework/zend-feed#75](https://github.com/zendframework/zend-feed/pull/75) deprecates each of:
  - `Laminas\Feed\Reader\Extension\Podcast\Entry::getKeywords()`
  - `Laminas\Feed\Reader\Extension\Podcast\Feed::getKeywords()`
  - `Laminas\Feed\Writer\Extension\ITunes\Entry::setKeywords()`
  - `Laminas\Feed\Writer\Extension\ITunes\Feed::setKeywords()`
  as the iTunes Podcast RSS specification no longer supports keywords.

### Removed

- Nothing.

### Fixed

- Nothing.

## 2.9.1 - 2018-05-14

### Added

- Nothing.

### Changed

- [zendframework/zend-feed#16](https://github.com/zendframework/zend-feed/pull/16) updates the `Laminas\Feed\Pubsubhubbub\AbstractCallback` to no longer use the
  `$GLOBALS['HTTP_RAW_POST_DATA']` value as a fallback when `php://input` is
  empty. The fallback existed because, prior to PHP 5.6, `php://input` could
  only be read once. As we now require PHP 5.6, the fallback is unnecessary,
  and best removed as the globals value is deprecated.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-feed#68](https://github.com/zendframework/zend-feed/pull/68) fixes the behavior of `Laminas\Feed\Writer\AbstractFeed::setTitle()` and
  `Laminas\Feed\Writer\Entry::setTitle()` to accept the string `"0"`.

- [zendframework/zend-feed#68](https://github.com/zendframework/zend-feed/pull/68) updates both `Laminas\Feed\Writer\AbstractFeed` and `Laminas\Feed\Writer\Entry`
  to no longer throw an exception for entry titles which have a string value of `0`.

## 2.9.0 - 2017-12-04

### Added

- [zendframework/zend-feed#52](https://github.com/zendframework/zend-feed/pull/52) adds support for PHP
  7.2

- [zendframework/zend-feed#53](https://github.com/zendframework/zend-feed/pull/53) adds a number of
  additional aliases to the `Writer\ExtensionPluginManager` to ensure plugins
  will be pulled as expected.

- [zendframework/zend-feed#63](https://github.com/zendframework/zend-feed/pull/63) adds the feed title
  to the attributes incorporated in the `FeedSet` instance, per what was already
  documented.

- [zendframework/zend-feed#55](https://github.com/zendframework/zend-feed/pull/55) makes two API
  additions to the `StandaloneExtensionManager` implementations of both the reader
  and writer subcomponents:

  - `$manager->add($name, $class)` will add an extension class using the
    provided name.
  - `$manager->remove($name)` will remove an existing extension by the provided
    name.

### Changed

- Nothing.

### Deprecated

- Nothing.

### Removed

- [zendframework/zend-feed#52](https://github.com/zendframework/zend-feed/pull/52) removes support for
  HHVM.

### Fixed

- [zendframework/zend-feed#50](https://github.com/zendframework/zend-feed/pull/50) fixes a few issues
  in the PubSubHubbub `Subscription` model where counting was being performed on
  uncountable data; this ensures the subcomponent will work correctly under PHP
  7.2.

## 2.8.0 - 2017-04-02

### Added

- [zendframework/zend-feed#27](https://github.com/zendframework/zend-feed/pull/27) adds a documentation
  chapter demonstrating wrapping a PSR-7 client to use with `Laminas\Feed\Reader`.
- [zendframework/zend-feed#22](https://github.com/zendframework/zend-feed/pull/22) adds missing
  ExtensionManagerInterface on Writer\ExtensionPluginManager.
- [zendframework/zend-feed#32](https://github.com/zendframework/zend-feed/pull/32) adds missing
  ExtensionManagerInterface on Reader\ExtensionPluginManager.

### Deprecated

- Nothing.

### Removed

- [zendframework/zend-feed#38](https://github.com/zendframework/zend-feed/pull/38) dropped php 5.5
  support

### Fixed

- [zendframework/zend-feed#35](https://github.com/zendframework/zend-feed/pull/35) fixed
  "A non-numeric value encountered" in php 7.1
- [zendframework/zend-feed#39](https://github.com/zendframework/zend-feed/pull/39) fixed protocol
  relative link absolutisation
- [zendframework/zend-feed#40](https://github.com/zendframework/zend-feed/pull/40) fixed service
  manager v3 compatibility aliases in extension plugin managers

## 2.7.0 - 2016-02-11

### Added

- [zendframework/zend-feed#21](https://github.com/zendframework/zend-feed/pull/21) edits, revises, and
  prepares the documentation for publication at https://docs.laminas.dev/laminas-feed/

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-feed#20](https://github.com/zendframework/zend-feed/pull/20) makes the two
  laminas-servicemanager extension manager implementations forwards compatible
  with version 3, and the overall code base forwards compatible with laminas-stdlib
  v3.

## 2.6.0 - 2015-11-24

### Added

- [zendframework/zend-feed#13](https://github.com/zendframework/zend-feed/pull/13) introduces
  `Laminas\Feed\Writer\StandaloneExtensionManager`, an implementation of
  `Laminas\Feed\Writer\ExtensionManagerInterface` that has no dependencies.
  `Laminas\Feed\Writer\ExtensionManager` now composes this by default, instead of
  `Laminas\Feed\Writer\ExtensionPluginManager`, for managing the various feed and
  entry extensions. If you relied on `ExtensionPluginManager` previously, you
  will need to create an instance manually and inject it into the `Writer`
  instance.
- [zendframework/zend-feed#14](https://github.com/zendframework/zend-feed/pull/14) introduces:
  - `Laminas\Feed\Reader\Http\HeaderAwareClientInterface`, which extends
    `ClientInterface` and adds an optional argument to the `get()` method,
    `array $headers = []`; this argument allows specifying request headers for
    the client to send. `$headers` should have header names for keys, and the
    values should be arrays of strings/numbers representing the header values
    (if only a single value is necessary, it should be represented as an single
    value array).
  - `Laminas\Feed\Reader\Http\HeaderAwareResponseInterface`, which extends
    `ResponseInterface` and adds the method `getHeader($name, $default = null)`.
    Clients may return either a `ResponseInterface` or
    `HeaderAwareResponseInterface` instance.
  - `Laminas\Feed\Reader\Http\Response`, which is an implementation of
    `HeaderAwareResponseInterface`. Its constructor accepts the status code,
    body, and, optionally, headers.
  - `Laminas\Feed\Reader\Http\Psr7ResponseDecorator`, which is an implementation of
    `HeaderAwareResponseInterface`. Its constructor accepts a PSR-7 response
    instance, and the various methdos then proxy to those methods. This should
    make creating wrappers for PSR-7 HTTP clients trivial.
  - `Laminas\Feed\Reader\Http\LaminasHttpClientDecorator`, which decorates a
    `Laminas\Http\Client` instance, implements `HeaderAwareClientInterface`, and
    returns a `Response` instance seeded from the laminas-http response upon
    calling `get()`. The class exposes a `getDecoratedClient()` method to allow
    retrieval of the decorated laminas-http client instance.

### Deprecated

- Nothing.

### Removed

- Nothing.

### Fixed

- [zendframework/zend-feed#5](https://github.com/zendframework/zend-feed/pull/5) fixes the enclosure
  length check to allow zero and integer strings.
- [zendframework/zend-feed#2](https://github.com/zendframework/zend-feed/pull/2) ensures that the
  routine for "absolutising" a link in `Reader\FeedSet` always generates a URI
  with a scheme.
- [zendframework/zend-feed#14](https://github.com/zendframework/zend-feed/pull/14) makes the following
  changes to fix behavior around HTTP clients used within
  `Laminas\Feed\Reader\Reader`:
  - `setHttpClient()` now ensures that the passed client is either a
    `Laminas\Feed\Reader\Http\ClientInterface` or `Laminas\Http\Client`, raising an
    `InvalidArgumentException` if neither. If a `Laminas\Http\Client` is passed, it
    is passed to the constructor of `Laminas\Feed\Reader\Http\LaminasHttpClientDecorator`,
    and the decorator instance is used.
  - `getHttpClient()` now *always* returns a `Laminas\Feed\Reader\Http\ClientInterface`
    instance. If no instance is currently registered, it lazy loads a
    `LaminasHttpClientDecorator` instance.
  - `import()` was updated to consume a `ClientInterface` instance; when caches
    are in play, it checks the client against `HeaderAwareClientInterface` to
    determine if it can check for HTTP caching headers, and, if so, to retrieve
    them.
  - `findFeedLinks()` was updated to consume a `ClientInterface`.
