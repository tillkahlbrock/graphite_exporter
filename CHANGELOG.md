# unreleased

* [ENHANCEMENT] Log incoming and parsed samples if debug logging is enabled ([#58](https://github.com/prometheus/graphite_exporter/pull/58))

# 0.3.0 / 2018-08-22

This release contains two major breaking changes:

Flags now require two dashes (`--help` instead of `-help`).

The configuration format is now YAML, and uses the same format as the [statsd exporter](https://github.com/prometheus/statsd_exporter), minus support for
metric types other than gauges.
There is a [conversion tool](https://github.com/bakins/statsd-exporter-convert) available.
This change adds new features to the mappings:
It is now possible to specify the "name" label.
Regular expressions can be used to match on Graphite metric names beyond extracting dot-separated components.

* [CHANGE] Use YAML configuration format and mapper from statsd exporter ([#52](https://github.com/prometheus/graphite_exporter/pull/52))
* [CHANGE] Switch to the Kingpin flag library ([#30](https://github.com/prometheus/graphite_exporter/30))
* [FEATURE] Add metric for the sample expiry setting ([#34](https://github.com/prometheus/graphite_exporter/34))
* [FEATURE] Add pprof endpoint ([#33](https://github.com/prometheus/graphite_exporter/33))
* [BUGFIX] Accept whitespace around the Graphite protocol lines ([#53](https://github.com/prometheus/graphite_exporter/53))

# 0.2.0 / 2017-03-01

* [FEATURE] Added flag to allow dropping of unmatched metrics
* [ENHANCEMENT] Logging changes and standardisation


# 0.1.0 / 2015-05-05

Initial release.
