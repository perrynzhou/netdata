<!--
title: "Install Netdata with .deb/.rpm packages"
desciption: "Install the Netdata Agent with Linux packages that support Ubuntu, Debian, Fedora, RHEL, CentOS, openSUSE, and more."
custom_edit_url: https://github.com/netdata/netdata/edit/master/packaging/installer/methods/packages.md
-->

# Install Netdata with .deb/.rpm packages

![](https://raw.githubusercontent.com/netdata/netdata/master/web/gui/images/packaging-beta-tag.svg?sanitize=true)

Netdata provides our own flavour of binary packages for the most common operating systems that use with `.deb` and
`.rpm` packaging formats.

We provide two separate repositories, one for our stable releases and one for our nightly releases. Visit the repository
pages and follow the quick set-up instructions to get started.

1.  Stable releases: Our stable production releases are hosted in the 
    [netdata/netdata](https://packagecloud.io/netdata/netdata) repository on packagecloud
2.  Nightly releases: Our latest releases are hosted in the
    [netdata/netdata-edge](https://packagecloud.io/netdata/netdata-edge) repository on packagecloud

## Using caching proxies with packagecloud repositories

packagecloud only provides HTTPS access to repositories they host, which means in turn that Netdata's package
repositories are only accessible via HTTPS. This is known to cause issues with some setups that use a caching proxy for
package downloads.

If you are using such a setup, there are a couple of ways you can work around this:

-   Configure your proxy to automatically pass through HTTPS connections without caching them. This is the simplest
    solution, but means that downloads of Netdata pacakges will not be cached.
-   Mirror the respository locally on your proxy system, and use that mirror when installing on other systems. This
    requires more setup and more disk space on the caching host, but it lets you cache the packages locally.
-   Some specific caching proxies may have alternative configuration options to deal with these issues. You can find
    such options in their documentation.

## What's next?

When you finish installing Netdata, be sure to visit our [step-by-step guide](/docs/guides/step-by-step/step-00.md) for
a fully-guided tour into Netdata's capabilities and how to configure it according to your needs. 

Or, if you're a monitoring and system administration pro, skip ahead to our [getting started
guide](/docs/getting-started.md) for a quick overview.
