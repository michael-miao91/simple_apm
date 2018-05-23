# 开发中……
# SimpleApm
基于Redis的简单的Web请求性能监控/慢事务追踪工具

以天为维度记录：
- 最慢的1000个(默认1000)请求
- 记录每个action最慢的100次请求
- 记录每个action的平均访问时间
- 记录每个小时请求量
- 记录慢请求的详情和对应SQL详情（多余的会删掉）
- 以10分钟为刻度记录平均/最慢访问时间、次数等性能指标

## Usage

```ruby
# routes.rb
mount SimpleApm::Engine => '/apm'
```


## Installation
Add this line to your application's Gemfile:

```ruby
gem 'simple_apm'
```

And then execute:
```bash
$ bundle
```

Or install it yourself as:
```bash
$ gem install simple_apm
```

## Contributing
Contribution directions go here.

## License
The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).