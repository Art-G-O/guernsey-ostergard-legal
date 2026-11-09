# Guernsey-Ostergard legal pages

Static pages served at **https://legal.guernseyostergard.com** via GitHub Pages:

- `/privacy-policy/`
- `/terms-and-conditions/`

## Why this exists

US mobile carriers require a publicly reachable privacy policy and terms page
before a business may send text messages (A2P 10DLC campaign registration).
These two URLs are what the Twilio campaign registration points at. They back
the employee safety text message program, which delivers the weekly safety
topic each employee must read and acknowledge under WAC 296-155-110.

They live here rather than in the main WordPress site because admin access to
that site was not available when the campaign had to be registered. If the
pages are later moved onto guernseyostergard.com, update the URLs in the Twilio
campaign first, then retire this repo.

## Do not remove without checking

Three things must survive any edit or the carrier registration can be revoked:

1. The privacy page must be titled "Privacy Policy".
2. It must name Guernsey-Ostergard Painting LLC.
3. It must contain this sentence, in these exact words:
   *"We do not sell or share your SMS opt-in data or personal information with
   third parties for marketing purposes"*

The terms page must keep its title, the company name, the message frequency,
"Message and data rates may apply", and the STOP and HELP instructions.

## DNS

`legal.guernseyostergard.com` is a CNAME to `art-g-o.github.io`. DNS for the
domain is managed by Zypes. The `CNAME` file in this repo tells GitHub Pages
which hostname to answer on - do not delete it.

Source copies of the text are kept with the Safety Signoff project.
