=== Merged Comments for WPML ===
Contributors: CodingFabian, simonwheatley, jeangalea, poonasor
Donate link: https://rickypoon.ca/
Tags: WPML, comments, multilingual, translation, i18n
Requires at least: 2.7
Tested up to: 6.0.1
Stable tag: 3.0
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

An updated version of the fixed version of the no longer maintained WPML Comment Merging plugin.

== Description ==

Because WPML creates posts and pages for each language, comments from one do not appear on the other.

This plugin merges comments from all WPML translations of the posts and pages, so that they all are displayed on each other.
Comments are internally still attached to the post or page they were made on.

It uses the `get_comments()` api call, which in some circumstances might not return all posts.

This is a fixed version of the no longer maintained WPML Comment Merging plugin:
[http://wordpress.org/extend/plugins/wpml-comment-merging/](http://wordpress.org/extend/plugins/wpml-comment-merging/ "wpml-comment-merging")

Thanks to Simon Wheatley for contributing the fix.

Forked from: [https://github.com/jgalea/wpml-comments-merging](https://github.com/jgalea/wpml-comments-merging/ "Github")

== Frequently Asked Questions ==

= What types of content are supported =

Initially only posts were supported, but since 1.2 also pages are supported.

= Does it work with the WPML auto translation? =

It should, but I have not tested it. It hooks in after the WPML hooks (using prio 100) and uses the comments passed to it.

== Changelog ==

= 3.0 =
* Updated version 2.5, added $sitepress class and removed comments_clauses filter to allow to display multiple languages 

= 2.5 =
* Fixed the no-longer maintained version.

= 1.3 =
* Fix for regression in PHP breaking call_user_func calls ( Warning: Parameter 1 to get_post() expected to be a reference, value given in line 45 of wpml-comment-merging.php )

= 1.2 =
* Added support for merging comments on pages.

= 1.1 =
* Fixed issue with comment counting on start page when a post is not translated

= 1.0 =
* Initial Release
