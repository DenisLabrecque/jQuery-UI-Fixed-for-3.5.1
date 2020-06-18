# Fix jQuery 3.5.1 Migrate Warnings for jQuery UI 1.12.1
jQuery UI releases have gone stagnant since 2017. For that reasons, they contain deprecations of jQuery. The goal of this is just to correct those statements that need fixing, and change nothing else. These are the warnings:

    jquery-migrate-3.3.0.js:100 JQMIGRATE: jQuery.expr[':'] is deprecated; use jQuery.expr.pseudos

    JQMIGRATE: jQuery.expr.filters is deprecated; use jQuery.expr.pseudos

    JQMIGRATE: jQuery.isArray is deprecated; use Array.isArray

    JQMIGRATE: jQuery.isFunction() is deprecated

According to a [discussion thread](https://github.com/jquery/jquery/commit/1b9575b9d14399e9426b9eacdd92b3717846c3f2), this is already done in UI code, but is not included in a single release.

Use this code at your own risk. Though every effort has been made to write correct changes, I do not know how to test them fully.
