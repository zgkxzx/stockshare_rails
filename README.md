== 是一个我为朋友做的一个库存管理系统，我选择在一开始就开源，欢迎正在学习Rails的同学一起共同进步。
我是根据这个Guide先走了一遍，这个Guide的质量还是比较高。比较顺利。
 > [http://guides.rubyonrails.org/getting_started.html]

注册，登陆用的这个Guide:
 > [http://guides.railsgirls.com/devise/]

在中国大陆因为有防火墙的原因所以Rails开始比较困难。
 > `gem install` 设置代理的命令如下：
 > `gem install -p http://10.10.10.10:8080 rails`
 
你需要有一个http的代理，这里的`10.10.10.10:8080`只是一个例子。

Bundle install 设置代理在执行前先:
 > Windows:`SET http_proxy=http://10.10.10.10:8080`
 
 > Mac:`EXPORT http_proxy=http://10.10.10.10:8080`

理解CanCan:http://blog.xdite.net/posts/2012/07/30/cancan-rule-engine-authorization-based-library-1/
写的很好，迷茫了一天的看看算清楚了。

另外CanCan不支持rails4了，使用CanCanCan解决。

* Ruby version
 > 我用的是Rails 4.2.1

* System dependencies

* Configuration

* Database creation

Development环境执行:
 > `rake db:migrate`

Production环境执行：
 > `rake db:migrate RAILS_ENV=production`

* How to run the test suite

Development环境执行：
 > `rails server`

Production环境执行我的是在DigitalOcean上面，Nginx + Unicorn  + Rails：
 > `RAILS_ENV=production rake assets:precompile`
 > `/etc/init.d/unicorn restart`
 
* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions
install http://www.imagemagick.org/script/binary-releases.php

* ...


Please feel free to use a different markup language if you do not plan to run
<tt>rake doc:app</tt>.

[http://guides.rubyonrails.org/getting_started.html]: http://guides.rubyonrails.org/getting_started.html
[http://guides.railsgirls.com/devise/]: http://guides.railsgirls.com/devise/
