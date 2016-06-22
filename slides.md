# High Availability

---

* LAMP Stack
* Database
* Mail Server
* NFS Server
* Virtual Machines
* Containers
* Custom Applications
* ...

---

### Using High Availability is **easy** on openSUSE.

---

#### **Hawk** is a web interface for High Availability clusters based on Pacemaker and corosync.

---

## Installation
##### Leap, Tumbleweed

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

<img src="img/trainwreck2.jpg">

---

* Rails 4.2
* Twitter Bootstrap 3
* JsRender / JsViews
* HAML, YAML, SCSS, ...

---

<img src="img/puma-logo-large.png" >

---

# Packaging gems

* `devel:languages:ruby:extensions`
* `gem2rpm`

---

## Tumbleweed moves fast

1. `rubygem-arel` is updated from v. 6 to 7
2. `rails` is now unresolvable (requires 6)
3. `hawk` is now unresolvable...

---

### Re-packaging

`rubygem-arel` to `rubygem-arel-6`

---

Changes can take a long time to trickle into Tumbleweed.

---

## OBS and Package Managers

* Packaging language-specific packages as `rpm` is painful
* gem-aware zypper + obs, generate needed rpms from gem + gem2rpm.yml
  on install?

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
