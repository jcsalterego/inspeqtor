# Inspeqtor Changelog

Inspeqtor is brand new software; it very likely has bugs.
Try it out and let us know how we can improve it for you.

Version 1.0 will be released when it is stable and ready for widespread usage.

See [Current Release Status](https://github.com/mperham/inspeqtor/milestones) here.

## 0.6.0

- Add [init.d](https://github.com/mperham/inspeqtor/wiki/Initd) support [#14]
- Add new "export" command to emit current metric values as JSON [#2]
- Send metrics to [Statsd](https://github.com/mperham/inspeqtor/wiki/Pro-Statsd) [#2] **Pro**
- Monitor [cron job execution](https://github.com/mperham/inspeqtor/wiki/Pro-Recurring-Jobs) [#5] **Pro**
- Support per-second rates for thresholds [#11]
```bash
  # Use the "/sec" suffix. You can use the k,m,g modifier letters also.
  if mysql:Queries > 1k/sec then alert
  if mysql:Slow_queries > 1/sec then alert
```
- Changed the /etc/inspeqtor layout a bit [#22]
- inspeqtorctl no longer requires sudo for members of the 'adm' group [#27]

## 0.5.0

- Initial Release
- Yay, shipped it!
