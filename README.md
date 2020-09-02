你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
[![Travis](https://travis-ci.org/elastic/beats.svg?branch=master)](https://travis-ci.org/elastic/beats)
[![GoReportCard](http://goreportcard.com/badge/elastic/beats)](http://goreportcard.com/report/elastic/beats)
[![codecov.io](https://codecov.io/github/elastic/beats/coverage.svg?branch=master)](https://codecov.io/github/elastic/beats?branch=master)

# Beats - The Lightweight Shippers of the Elastic Stack

The [Beats](https://www.elastic.co/products/beats) are lightweight data
shippers, written in Go, that you install on your servers to capture all sorts
of operational data (think of logs, metrics, or network packet data). The Beats
send the operational data to Elasticsearch, either directly or via Logstash, so
it can be visualized with Kibana.

By "lightweight", we mean that Beats have a small installation footprint, use
limited system resources, and have no runtime dependencies.

This repository contains
[libbeat](https://github.com/elastic/beats/tree/master/libbeat), our Go
framework for creating Beats, and all the officially supported Beats:

Beat  | Description
--- | ---
[Auditbeat](https://github.com/elastic/beats/tree/master/auditbeat) | Collect your Linux audit framework data and monitor the integrity of your files.
[Filebeat](https://github.com/elastic/beats/tree/master/filebeat) | Tails and ships log files
[Heartbeat](https://github.com/elastic/beats/tree/master/heartbeat) | Ping remote services for availability
[Metricbeat](https://github.com/elastic/beats/tree/master/metricbeat) | Fetches sets of metrics from the operating system and services
[Packetbeat](https://github.com/elastic/beats/tree/master/packetbeat) | Monitors the network and applications by sniffing packets
[Winlogbeat](https://github.com/elastic/beats/tree/master/winlogbeat) | Fetches and ships Windows Event logs

In addition to the above Beats, which are officially supported by
[Elastic](https://elastic.co), the community has created a set of other Beats
that make use of libbeat but live outside of this Github repository. We maintain
a list of community Beats
[here](https://www.elastic.co/guide/en/beats/libbeat/master/community-beats.html).

## Documentation and Getting Started

You can find the documentation and getting started guides for each of the Beats
on the [elastic.co site](https://www.elastic.co/guide/):

* [Beats platform](https://www.elastic.co/guide/en/beats/libbeat/current/index.html)
* [Auditbeat](https://www.elastic.co/guide/en/beats/auditbeat/current/index.html)
* [Filebeat](https://www.elastic.co/guide/en/beats/filebeat/current/index.html)
* [Heartbeat](https://www.elastic.co/guide/en/beats/heartbeat/current/index.html)
* [Metricbeat](https://www.elastic.co/guide/en/beats/metricbeat/current/index.html)
* [Packetbeat](https://www.elastic.co/guide/en/beats/packetbeat/current/index.html)
* [Winlogbeat](https://www.elastic.co/guide/en/beats/winlogbeat/current/index.html)


## Getting Help

If you need help or hit an issue, please start by opening a topic on our
[discuss forums](https://discuss.elastic.co/c/beats). Please note that we
reserve GitHub tickets for confirmed bugs and enhancement requests.

## Downloads

You can download pre-compiled Beats binaries, as well as packages for the
supported platforms, from [this page](https://www.elastic.co/downloads/beats).

## Contributing

We'd love working with you! You can help make the Beats better in many ways:
report issues, help us reproduce issues, fix bugs, add functionality, or even
create your own Beat.

Please start by reading our [CONTRIBUTING](CONTRIBUTING.md) file.

If you are creating a new Beat, you don't need to submit the code to this
repository. You can simply start working in a new repository and make use of the
libbeat packages, by following our [developer
guide](https://www.elastic.co/guide/en/beats/libbeat/current/new-beat.html).
After you have a working prototype, open a pull request to add your Beat to the
list of [community
Beats](https://github.com/elastic/beats/blob/master/libbeat/docs/communitybeats.asciidoc).

## Building Beats from the Source

See our [CONTRIBUTING](CONTRIBUTING.md) file for information about setting up
your dev environment to build Beats from the source.
