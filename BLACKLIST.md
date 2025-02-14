#########################################################################
# PROCMAIL BLACKLIST FOR MAIL ACCOUNTS @Version 1.0 - 02/2025
# -----------------------------------------------------------------------
# @Author: Rick Armann
# @Author URI: https://wunderheit.de
#########################################################################
# This Procmail rule helps to filter spam emails from specific domains
# and move them directly to the spam folder.
#
# Optimized for All-Inkl Mail Accounts.
#
# How to use:
# 1. Log in to your All-Inkl Webmail.
# 2. Go to Settings > Procmail Editor.
# 3. Copy and paste the following rule into the editor.
# 4. Save and test.
#########################################################################

# Blacklist Rule (Move to Spam)

:0 H:
* ^From:.*@(aberwell\.com|aklessos\.com|pasliko\.com|abergless\.com|gaholters\.com|xulioos\.com|gehetess\.com|xallower\.com|couponslabs\.net|usequote\.net|guteswell\.com|centrohara\.it|pureleto\.com|sichere-anlage\.com|tagerliss\.com|yalberto\.com|interssant\.com|xansers\.com|zeriogom\.com|solpuress\.com|terlikass\.com)
| $DELIVER -m "Spam"