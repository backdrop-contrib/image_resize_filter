Image Resize Filter
===================

This filter automatically resizes images to their width and height dimensions.
Users never have to worry about uploading pre-sized images again; they can just
insert an image, set it's width and height properties, and the image is
automatically resized on output.

Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules

- Visit the configuration page under Administration > Configuration > Content
  authoring > Text editors and formats (admin/config/content/formats) and click
  'Configure' next to the text editor you want the image resize filter enabled
  for.

- Check the box for 'Image resize filter' under the list of filters.

- IMPORTANT: Re-order your enabled filters under 'Filter processing order'.

  If using the Image Resize Filter on the 'Filtered HTML' text editor, you MUST
  ensure:
    1. That the `<img>` tag is in the list of allowed tags, and
    2. That the 'Image resize filter' is run BEFORE the 'HTML filter'.

  If using the Image Resize Filter with BBCode or some other non-HTML filter,
  the 'Image resize filter' must be run AFTER the BBCode filter. If using
  Pathologic (https://backdropcms.org/project/pathologic), Image Resize Filter
  must be run AFTER the Pathologic filter too, since Pathologic must correct
  image path locations for Image Resize Filter to find the images.

- Optional: Click the Image resize filter tab underneath 'Filter settings' to
  set additional configuration for the the image resize filter.

Issues
------

Bugs and Feature requests should be reported in the Issue Queue:
https://github.com/backdrop-contrib/image_resize_filter/issues

It is important to understand that Image Resize Filter has absolutely no effect
on the content creation form. If you are having trouble resizing an image in an
editor or editing a piece of content, DO NOT file an issue with Image Resize
Filter. This module is only responsible for the display of output and has
absolutely no effect on editing or creating new content.

Credits
-------

- Ported to Backdrop CMS by Peter Anderson (https://github.com/BWPanda).
- Originally written for Drupal by Nathan Haug (https://github.com/quicksketch).

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.

