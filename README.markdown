# [Mail MIME](http://drupal.org/project/mailmime)

Provides a class for creating MIME messages.

*   *NOTE: This module does not send mail.*

    :   If you came here looking for a mail-sending module, try
        [HTML Mail](http://drupal.org/project/htmlmail) (which can use this
        module for MIME-handling) or
        [Mime Mail](http://drupal.org/project/mimemail) (which comes with its
        own MIME-handling library).

[Mail Mime](http://drupal.org/project/mailmime) extends the
[PEAR](http://pear.php.net/) class called
[Mail_Mime](http://pear.php.net/package/Mail_Mime)
*(version 1.6.1 or later)* to provide a
drupal-friendly library for creating and parsing MIME messages.  Neither
[Mail Mime](http://drupal.org/project/mailmime) nor
[Mail_Mime](http://pear.php.net/package/Mail_Mime) send mail nor do anything
useful on their own.  Both are intended as code libraries to be used by *other*
programs that send or receive mail.

[Mail Mime](http://drupal.org/project/mailmime) started out as part of
[HTML Mail](http://drupal.org/project/htmlmai).  I separated into its own
module for two reasons:

1.  The separation helped clarify in my own mind which parts of the mail-sending
    process require MIME and which do not.  The resulting code is simpler and
    easier to maintain.

2.  It is possible that another mail-sending or mail-reading module may find the
    [Mail Mime](http://drupal.org/project/mailmime) library useful.

## [Requirement](http://www.dict.org/bin/Dict?Form=Dict2&Database=*&Query=requirement)

Either:

:   *   The [PEAR](http://pear.php.net/) package called
        [Mail_Mime](http://pear.php.net/package/Mail_Mime) must be installed and
        available somewhere on the
        [`include_path`](http://php.net/manual/ini.core.php#ini.include-path).

Or:

:   *   If the [Mail_Mime](http://pear.php.net/package/Mail_Mime) is not
        available, the [Include](http://drupal.org/project/include) module
        can automatically download and enable the required files.

## [Installation](http://drupal.org/documentation/install/modules-themes/modules-5-6)

1.  Download and install
    [as usual](http://drupal.org/documentation/install/modules-themes/modules-5-6).

2.  When enabled, [Mail Mime](http://drupal.org/project/mailmime) will

    *   Auto-detect whether the required files are present.

    *   If any files are missing, and the
        [Include](http://drupal.org/project/include) module is available,
        [Mail Mime](http://drupal.org/project/mailmime) will use
        [Include](http://drupal.org/project/include) to auto-download and
        enable the missing files.

    *   If all of the above fails,
        [Mail Mime](http://drupal.org/project/mailmime) will disable itself
        and print a warning to both the screen and the error log.
