# ProcessWire starter

My repo for experimenting with ProcessWire.

For the full official README: https://github.com/processwire/processwire/blob/master/README.md

Startup short version:

1. Is Apache running?

   - `apache2ctl status` to check
   - `sudo apache2ctl start` to fire it up
   - `apache2ctl stop` and `apache2ctl restart` if there's a problem

2. Is MySQL running?

   - `mysql.server status` to check
   - `mysql.server start` if it isn't

3. Is the PHP server running?
   - `php -S localhost:3033`

## Table of Contents

- [Installation](#installing-processwire)
- [Upgrading](#upgrading-processwire)
- [Troubleshooting](https://processwire.com/docs/start/install/troubleshooting/)
- [Support](#support-and-links)

### Reference

- [ProcessWire website](https://processwire.com)
- [About ProcessWire](https://processwire.com/about/)
- [Support forums](https://processwire.com/talk/)
- [Documentation](https://processwire.com/docs/)
- [API reference](https://processwire.com/api/ref/)
- [Downloads](https://processwire.com/download/)
- [Modules/plugins](https://processwire.com/modules/)
- [Showcase](https://processwire.com/sites/)

---

## Installing ProcessWire

Simply extract the ProcessWire files to an http accessible location and
load the URL in your web browser. This will start the installer. See our
[Installation Guide](https://processwire.com/docs/start/install/new/) for more
details and instructions. If you run into any trouble, please see our
[Troubleshooting Guide](https://processwire.com/docs/start/install/troubleshooting/).

## Upgrading ProcessWire

Upgrading is easy and usually just a matter of replacing your `/wire/` directory
with the one from the new version. But to be safe, before proceeding with any version upgrade, please see the
[Upgrading ProcessWire](https://processwire.com/docs/start/install/upgrade/)
guide and perhaps keep it open during your upgrade in case you need to refer back to it.

When upgrading from one 3.x version to another, please use the
[general upgrade process](https://processwire.com/docs/start/install/upgrade/#general-upgrade-process).
This consists primarily of making sure you've got everything backed up and then just
replacing your `/wire/` directory with the one from the newer version.

- If you are upgrading from a 3.x version prior to 3.0.135 then please also follow
  [these instructions](https://processwire.com/docs/start/install/upgrade/from-3.x/).

- If you are upgrading from any 2.x version then please see
  [upgrading from ProcessWire 2.x](https://processwire.com/docs/start/install/upgrade/from-2.x/).

- If you run into any trouble upgrading, please see our
  [troubleshooting upgrades guide](https://processwire.com/docs/start/install/troubleshooting/#troubleshooting-upgrades).

## Debug Mode

Debug mode causes all errors to be reported to the screen. This can be
helpful during development or troubleshooting. When in the admin, it also
enables a “Debug” link (see footer) for reporting of extra information in a
panel. Debug mode is not intended for live or production sites, as the
information reported is for the developer only. Do not leave debug mode
on for any live/production sites, as it could be a security concern. However,
we think you'll find it very handy during development or when resolving issues.

1. Edit this file: `/site/config.php`
2. Find this line: `$config->debug = false;`
3. Change the `false` to `true` like below, and save.

```
$config->debug = true;
```

This can be found near the bottom of the file, or you can add it if not
already there. It will make PHP and ProcessWire report all errors, warnings,
notices, etc. Of course, you'll want to set it back to false once you've
resolved any issues.

## Support and Links

- [ProcessWire Support Forums](https://processwire.com/talk/)
- [ProcessWire Weekly News](https://weekly.pw/)
- [ProcessWire Blog](https://processwire.com/blog/)
- [Sites running ProcessWire](https://processwire.com/sites/)
- [Subscribe to ProcessWire Weekly email](https://processwire.com/community/newsletter/subscribe/)
- [Submit your site to our directory](https://processwire.com/sites/submit/)
- [Follow @processwire on X-Twitter](http://twitter.com/processwire/)
- [Contact ProcessWire developer](https://processwire.com/contact/)
- [Report issue](https://github.com/processwire/processwire-issues/issues)

---

Copyright 2023 by Ryan Cramer / Ryan Cramer Design, LLC
