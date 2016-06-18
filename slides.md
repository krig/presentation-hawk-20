### Using High Availability is **easy** on openSUSE.

---

#### **Hawk** is a web interface for High Availability clusters based on Pacemaker and corosync.

---

* LAMP Stack
* Database
* NFS Server
* Virtual Machines
* Containers
* Custom Applications
* ...

---

## Installation

```bash
$ zypper install ha-cluster-bootstrap
$ ha-cluster-init
```

---

## Cluster Container

`github.com/krig/docker-hawk`

```bash
$ docker pull krig/hawk
```

---

`hawk-guide.readthedocs.io`

---

# **DEMO**

---

### Packaging a Ruby on Rails app for openSUSE

---

* Ruby on Rails
* Twitter Bootstrap
* bootstrap-table
* JsRender / JsViews
* Various other gems (HAML, YAML, SCSS, ...)

---

<img src="img/trainwreck2.jpg">

---

# Packaging gems

* `devel:languages:ruby:extensions`
* `gem2rpm`

---

### Tumbleweed moves fast = App breaks often

A lot of time spent managing `Gemfile`, re-packaging gems.

---

### Re-packaging gems

`rubygem-arel` to `rubygem-arel-6`

---

Re-packaging is easy, but packages can take a long time to trickle into Tumbleweed.

---

## gem hell

* `rubygem-mini_portile` = `0.6.2`
* `rubygem-mini_portile-2` = `2.1.0`
* `rubygem-mini_portile-2.0` = `2.0.0`
* `2.0.0.rc2` > `2.0.0` :(

---

## OBS and Package Managers

* Packaging language-specific packages as `rpm` is painful
* Is there a better way?

---

# Gem bundling

* Bundle correct gem versions in Hawk `.rpm`

* Solution for SLE HA

* Makes security updates cumbersome

---

# Future

---

## Things to fix

* Too faithful to Pacemaker

* JsViews vs. Rails views?

---

## Single Page Application

---

## Fewer dependencies

---

## Rust backend, JS frontend?
