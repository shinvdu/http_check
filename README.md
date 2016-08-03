A script to check list of live sites to teach if they are health. if only site is not, then make an email notification.

Rename  http_check.yaml.example to  http_check.yaml

make below config according to your own email, now it only surpport 163.mail.com

<pre>
    sender: "18217401108@163.com"
    pass: "xxxxx"
    # Recipients of the error report - in any valid format
    recipients: "sxie@altima-agency.cn"
    # The subject of the error report
    subject: "HTTP check error report"
</pre>


Config monitoring files, like below.

<pre>
sites:
- name: "GitHub"
  domain: "github.com"
  https: true

- name: "sky-city"
  domain: "blog.sky-city.me"
  https: true
  uri: "node/20"

- name: "sky-city"
  domain: "blog.sky-city.me"
  https: true
  uri: "node/2000"

</pre>


that is it.



