Basketballverse
v0.91.5 · Start Menu Restore

WHY THIS HAPPENED
The prior builds never permanently changed the startup heading/logo in the base HTML.
They relied on JavaScript after the page loaded to turn:
"Create a Basketballverse"
into:
"Create Your Universe"
and then insert the logo.

That meant if startup rendering happened before that patch, the old heading and no logo
could appear again.

FIX
- The startup logo is now written directly into the HTML.
- The heading is now written directly into the HTML as:
  Create Your Universe
- The runtime helper remains only as a backup and will not duplicate the logo.
- Removed the CSS rule that added its own white background behind the logo.

NOTE
The supplied logo file in this build is still the existing JPEG. A JPEG itself cannot
contain transparency; replacing it with a transparent PNG can be done separately.

FILES TO UPLOAD
- index.html
- basketballverse-logo.jpg
