v0.33.1 Basketball Universe — Create Universe Fix

BUG FIX
- Fixed Create Universe doing nothing in v0.33.
- The League File variable was declared too late in page startup.
- That caused the JavaScript to stop before the Create Universe button handler was attached.
- League File import/export and custom setup remain included.

No gameplay systems were changed in this hotfix.

GitHub update:
Upload index.html and README.txt over the current files and commit.
