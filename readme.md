# A WordPress Plugin Developers VVV

This is an [auto-site setup](https://github.com/Varying-Vagrant-Vagrants/VVV/wiki/Auto-site-Setup) designed to be used with [Varying Vagrants Vagrant](https://github.com/Varying-Vagrant-Vagrants/VVV) for development on the Yoast VideoSEO plugin.

## To get started:

1. Setup [Varying Vagrant Vagrants](https://github.com/Varying-Vagrant-Vagrants/VVV) (If you don't already have it)
2. Clone this repo into the www directory of your Vagrant as www/videoseo
3. Update to a [release tag](https://github.com/yoast/videoseo-vvv/releases) to keep stable
4. If your Vagrant is running, from the Vagrant directory run `vagrant halt`
5. Followed by `vagrant up --provision`.

Perhaps a cup of tea or coffee now? The provisioning may take a while.

Then you can visit [http://videoseo.dev/](http://videoseo.dev/) to start developing plugins.

## To start over (clean development environment):

You can do it the soft way using (I know it's long, Text Expander?) `vagrant ssh -c 'cd /home/vagrant/www/videoseo/ && rm -Rf htdocs/ && sh vvv-init.sh'`. Or, you can do it the hard way `vagrant reload --provision` and get a cup of coffee.

## Dependencies

- [Varying Vagrants Vagrant](https://github.com/Varying-Vagrant-Vagrants/VVV) - [Installation guide](https://github.com/Varying-Vagrant-Vagrants/VVV#the-first-vagrant-up)
- [vagrant-hostsupdater](https://github.com/cogitatio/vagrant-hostsupdater) - Install with `vagrant plugin install vagrant-hostsupdater`

## What will happen?

- Installs WordPress
- Installs a bunch of developer plugins
- Installs a bunch of plugins the VideoSEO plugin supports (or should support)

## Credentials and Such

### VideoSEO

* Username: `admin`
* Password: `password`
* Login: [login](http://videoseo.dev/wp-admin)

### MySQL Root

* User: `root`
* Pass: `root`
* See: [Connecting to MySQL](https://github.com/varying-vagrant-vagrants/vvv/wiki/Connecting-to-MySQL) from your local machine

_________________________

# Changelog

## 1.0

- Initial setup

_________________________

# Credits

Based on https://github.com/jrfnl/wordpress-plugins-tutorial
